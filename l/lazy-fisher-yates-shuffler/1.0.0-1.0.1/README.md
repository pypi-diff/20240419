# Comparing `tmp/lazy_fisher_yates_shuffler-1.0.0.tar.gz` & `tmp/lazy_fisher_yates_shuffler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_fisher_yates_shuffler-1.0.0.tar", max compression
+gzip compressed data, was "lazy_fisher_yates_shuffler-1.0.1.tar", max compression
```

## Comparing `lazy_fisher_yates_shuffler-1.0.0.tar` & `lazy_fisher_yates_shuffler-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10148 2024-04-17 21:16:40.098048 lazy_fisher_yates_shuffler-1.0.0/LICENSE
--rw-r--r--   0        0        0     1383 2024-04-17 21:55:00.901475 lazy_fisher_yates_shuffler-1.0.0/README.md
--rw-r--r--   0        0        0      688 2024-04-17 20:51:04.903549 lazy_fisher_yates_shuffler-1.0.0/lazy_fisher_yates_shuffler/__init__.py
--rw-r--r--   0        0        0     5845 2024-04-17 18:06:43.304925 lazy_fisher_yates_shuffler-1.0.0/lazy_fisher_yates_shuffler/bit_manager.py
--rw-r--r--   0        0        0     6087 2024-04-17 19:18:54.761512 lazy_fisher_yates_shuffler-1.0.0/lazy_fisher_yates_shuffler/persistence.py
--rw-r--r--   0        0        0    28757 2024-04-17 20:40:46.616967 lazy_fisher_yates_shuffler-1.0.0/lazy_fisher_yates_shuffler/shuffler.py
--rw-r--r--   0        0        0      412 2024-04-17 21:55:00.897302 lazy_fisher_yates_shuffler-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 lazy_fisher_yates_shuffler-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10148 2024-04-17 21:16:40.098048 lazy_fisher_yates_shuffler-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1383 2024-04-17 21:55:00.901475 lazy_fisher_yates_shuffler-1.0.1/README.md
+-rw-r--r--   0        0        0      688 2024-04-17 20:51:04.903549 lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/__init__.py
+-rw-r--r--   0        0        0     5845 2024-04-17 18:06:43.304925 lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/bit_manager.py
+-rw-r--r--   0        0        0     6087 2024-04-17 19:18:54.761512 lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/persistence.py
+-rw-r--r--   0        0        0    28815 2024-04-18 22:25:01.288051 lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/shuffler.py
+-rw-r--r--   0        0        0      412 2024-04-18 22:25:38.428455 lazy_fisher_yates_shuffler-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 lazy_fisher_yates_shuffler-1.0.1/PKG-INFO
```

### Comparing `lazy_fisher_yates_shuffler-1.0.0/LICENSE` & `lazy_fisher_yates_shuffler-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lazy_fisher_yates_shuffler-1.0.0/README.md` & `lazy_fisher_yates_shuffler-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lazy_fisher_yates_shuffler-1.0.0/lazy_fisher_yates_shuffler/__init__.py` & `lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_fisher_yates_shuffler-1.0.0/lazy_fisher_yates_shuffler/bit_manager.py` & `lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/bit_manager.py`

 * *Files identical despite different names*

### Comparing `lazy_fisher_yates_shuffler-1.0.0/lazy_fisher_yates_shuffler/persistence.py` & `lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/persistence.py`

 * *Files identical despite different names*

### Comparing `lazy_fisher_yates_shuffler-1.0.0/lazy_fisher_yates_shuffler/shuffler.py` & `lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/shuffler.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,87 +27,44 @@
 
 
 class _Node:
     """
     Node in binary tree for lazy Fisher-Yates shuffle.
     """
 
-    TERMINAL_SIZE: Final[int] = 64
-    """
-    Terminal size (number of bits in qword).
-    """
-
-    TERMINAL_SIZE_BITMASK: Final[int] = TERMINAL_SIZE - 1
-    """
-    Terminal size bitmask.
-    """
-
-    TERMINAL_SIZE_BIT_COUNT: Final[int] = TERMINAL_SIZE_BITMASK.bit_count()
-    """
-    Terminal size bit count.
-    """
-
-    TERMINAL_BIT_MANAGER: Final[BitManager] = BitManager(TERMINAL_SIZE)
-    """
-    Bit manager for terminal struck bitmap manipulation.
-    """
-
-    _BIT_COUNT_BITMASK_2: Final[int] = 0x5555555555555555
-    """
-    Bitmask for 2 binary digits bit count (even bits).
-    """
-
-    _BIT_COUNT_BITMASK_4: Final[int] = 0x3333333333333333
-    """
-    Bitmask for 4 binary digits bit count (even 2-bit groups).
-    """
-
-    _BIT_COUNT_BITMASK_8: Final[int] = 0x0F0F0F0F0F0F0F0F
-    """
-    Bitmask for 8 binary digits bit count (even nibbles).
-    """
-
-    def __init__(self, persistence_manager: PersistenceManager, bit_manager: BitManager, key: int, bit_number: int,
-                 restore: bool):
+    def __init__(self, shuffler: Shuffler, key: int, bit_number: int, restore: bool):
         """
         Construct a node.
 
-        :param persistence_manager: Persistence manager from shuffler.
-
-        :param bit_manager: Bit manager from shuffler.
+        :param shuffler: Enclosing shuffler.
 
         :param key: Persistence key for node state.
 
         :param bit_number: Bit number supported by this node.
 
         :param restore: If true, attempts to restore the node state.
         """
 
-        self.persistence_manager: Final[PersistenceManager] = persistence_manager
+        self.shuffler: Final[Shuffler] = shuffler
         """
-        Persistence manager from shuffler.
-        """
-
-        self.bit_manager: Final[BitManager] = bit_manager
-        """
-        Bit manager from shuffler.
+        Enclosing shuffler.
         """
 
         self.key: Final[int] = key
         """
         Persistence key for node state.
         """
 
         self.bit_number: Final[int] = bit_number
         """
         Bit number supported by this node.
         """
 
         # Terminal node supports up to TERMINAL_SIZE entries.
-        self.terminal: Final[bool] = bit_number == _Node.TERMINAL_SIZE_BIT_COUNT - 1
+        self.terminal: Final[bool] = bit_number == Shuffler._TERMINAL_SIZE_BIT_COUNT - 1
         """
         True if this node is a terminal node.
         """
 
         self.struck_count: int
         """
         Number of struck entries in or below this node.
@@ -115,15 +72,17 @@
 
         self.struck_bitmap: int
         """
         Bitmap of struck entries if this is a terminal node.
         """
 
         # Attempt to restore the node state if indicated.
-        node_state: Final[Optional[NodeState]] = self.persistence_manager.restore_node_state(key) if restore else None
+        node_state: Final[Optional[NodeState]] = shuffler.persistence_manager.restore_node_state(key)\
+            if restore else \
+            None
 
         if node_state is None:
             # Node has no struck count.
             self.struck_count = 0
             self.struck_bitmap = 0
         else:
             self.struck_count = node_state.struck_count
@@ -145,35 +104,25 @@
 
         :param key: Key.
 
         :return: Node.
         """
 
         # Right and/or left node will be persisted if this node has a non-zero struck count.
-        return _Node(self.persistence_manager, self.bit_manager, key, self.bit_number - 1, self.struck_count != 0)
-
-    def save_state(self):
-        """
-        Save node state to the persistence manager.
-        """
-
-        if self.struck_count != 0:
-            self.persistence_manager.save_node_state(self.key, NodeState(self.struck_count, self.struck_bitmap))
-        else:
-            self.persistence_manager.delete_node_state(self.key)
+        return _Node(self.shuffler, key, self.bit_number - 1, self.struck_count != 0)
 
     @property
     def right(self) -> _Node:
         """
         :return: Right node, constructed if necessary.
         """
 
         if self._right is None:
             # Right key is key-2^(bit_number+1).
-            self._right = self.init_right_left(self.key - self.bit_manager.bit(self.bit_number + 1))
+            self._right = self.init_right_left(self.key - self.shuffler.bit_manager.bit(self.bit_number + 1))
 
         return self._right
 
     @property
     def left(self) -> _Node:
         """
         :return: Left node, constructed if necessary.
@@ -181,168 +130,14 @@
 
         if self._left is None:
             # Left key is key-1.
             self._left = self.init_right_left(self.key - 1)
 
         return self._left
 
-    def strike(self, incremental_index: int) -> int:
-        """
-        Strike a number not yet struck.
-
-        :param incremental_index: Incremental index.
-
-        :return: True index.
-        """
-
-        index: int
-
-        if not self.terminal:
-            right: Final[_Node] = self.right
-
-            # Normalize index to right node by adding number of struck entries in right node.
-            right_normalized_index: Final[int] = incremental_index + right.struck_count
-
-            bit_manager: Final[BitManager] = self.bit_manager
-            bit_number: Final[int] = self.bit_number
-
-            # Index is in range of right node if this node's bit is clear.
-            if bit_manager.is_clear(right_normalized_index, bit_number):
-                # No adjustment necessary.
-                index = right.strike(incremental_index)
-            else:
-                # Index is in range of left node; clear bit to determine left incremental index and set bit on result to
-                # account for right index.
-                index = bit_manager.set(self.left.strike(bit_manager.clear(right_normalized_index, bit_number)),
-                                        bit_number)
-        else:
-            incremental_index_remaining: int = incremental_index
-
-            # These variables record the individual steps, except the last, of the bit count algorithm from Figure 5-2
-            # of Hacker's Delight, 2nd edition, by Henry S. Warren, Jr., to count the bits in the unstruck bitmap.
-
-            # Each variable contains the count of the named number of bits repeating up to the size of a long integer
-            # (e.g., bitCount4 contains 16 counts of 4-bit sets).
-
-            # Need to find an unstruck bit, so invert the struck bitmap to begin.
-            bit_count_1: Final[int] = self.struck_bitmap ^ _Node.TERMINAL_BIT_MANAGER.all_bits
-            bit_count_2: Final[int] = bit_count_1 - (bit_count_1 >> 0x01 & _Node._BIT_COUNT_BITMASK_2)
-            bit_count_4: Final[int] = ((bit_count_2 & _Node._BIT_COUNT_BITMASK_4) +
-                                       (bit_count_2 >> 0x02 & _Node._BIT_COUNT_BITMASK_4))
-            bit_count_8: Final[int] = (bit_count_4 + (bit_count_4 >> 0x04)) & _Node._BIT_COUNT_BITMASK_8
-            bit_count_16: Final[int] = bit_count_8 + (bit_count_8 >> 0x08)
-            bit_count_32: Final[int] = bit_count_16 + (bit_count_16 >> 0x10)
-
-            # Starting with the broadest bit count, each block does the following:
-            #
-            #   1. Shifts the bit count to the right to accommodate the shift, stored in the terminal index,determined
-            #      by the previous steps (does not apply to the first block).
-            #   2. Extracts the right-most bit count and compares it to the incremental index remaining.
-            #   3. If less than or equal, the incremental index remaining is to the left, so:
-            #       a. subtracts the right-most bit count from the incremental index remaining; and
-            #       b. adds the number of bits considered (using bitwise "or" as all numbers are powers of 2) to the
-            #          terminal index (first block does straight assignment).
-            #
-            # Although a loop would yield cleaner code, the unrolled loop is faster.
-
-            right_bit_count: int
-
-            # 32-bit bit count; mask limits count to 0-32.
-            right_bit_count = bit_count_32 & 0x3F
-            if right_bit_count <= incremental_index_remaining:
-                incremental_index_remaining -= right_bit_count
-                index = 0x20
-            else:
-                index = 0x00
-
-            # 16-bit bit count; mask limits count to 0-16.
-            right_bit_count = bit_count_16 >> index & 0x1F
-            if right_bit_count <= incremental_index_remaining:
-                incremental_index_remaining -= right_bit_count
-                index |= 0x10
-
-            # 8-bit bit count; mask limits count to 0-8.
-            right_bit_count = bit_count_8 >> index & 0x0F
-            if right_bit_count <= incremental_index_remaining:
-                incremental_index_remaining -= right_bit_count
-                index |= 0x08
-
-            # 4-bit bit count; mask limits count to 0-4.
-            right_bit_count = bit_count_4 >> index & 0x07
-            if right_bit_count <= incremental_index_remaining:
-                incremental_index_remaining -= right_bit_count
-                index |= 0x04
-
-            # 2-bit bit count; mask limits count to 0-2.
-            right_bit_count = bit_count_2 >> index & 0x03
-            if right_bit_count <= incremental_index_remaining:
-                incremental_index_remaining -= right_bit_count
-                index |= 0x02
-
-            # 1-bit bit count; mask limits count to 0-1.
-            right_bit_count = bit_count_1 >> index & 0x01
-            if right_bit_count <= incremental_index_remaining:
-                incremental_index_remaining -= right_bit_count
-                index |= 0x01
-
-            # Set bit to mark entry as struck.
-            self.struck_bitmap = _Node.TERMINAL_BIT_MANAGER.set(self.struck_bitmap, index)
-
-        # One entry in this node or a descendant has been struck.
-        self.struck_count += 1
-
-        self.save_state()
-
-        return index
-
-    def reserve(self, index: int):
-        """
-        Reserve an entry. This is used when values are generated in a cyclic pattern.
-
-        :param index: True index.
-        """
-
-        if not self.terminal:
-            # Index is in range of right node if this node's bit is clear.
-            if self.bit_manager.is_clear(index, self.bit_number):
-                self.right.reserve(index)
-            else:
-                self.left.reserve(index)
-        else:
-            # Set bit to mark entry as struck.
-            self.struck_bitmap = _Node.TERMINAL_BIT_MANAGER.set(self.struck_bitmap, index & _Node.TERMINAL_SIZE_BITMASK)
-
-        # One entry in this node or a descendant has been struck.
-        self.struck_count += 1
-
-        self.save_state()
-
-    def unreserve(self, index: int):
-        """
-        Unreserve an entry. This is used when values are generated in a cyclic pattern.
-
-        :param index: True index.
-        """
-
-        if not self.terminal:
-            # Index is in range of right node if this node's bit is clear.
-            if self.bit_manager.is_clear(index, self.bit_number):
-                self.right.unreserve(index)
-            else:
-                self.left.unreserve(index)
-        else:
-            # Clear bit to mark entry as unstruck.
-            self.struck_bitmap = _Node.TERMINAL_BIT_MANAGER.clear(self.struck_bitmap,
-                                                                  index & _Node.TERMINAL_SIZE_BITMASK)
-
-        # One entry in this node or a descendant has been unstruck.
-        self.struck_count -= 1
-
-        self.save_state()
-
     def validate_state(self, keys: [int], size: int, cyclic: bool):
         """
         Validate node, ensuring that struck count is consistent with right and left nodes (if not terminal) or with
         struck bitmap (if terminal). Used for testing.
 
         :param keys:
         :param size: Expected node size.
@@ -357,15 +152,15 @@
 
         if not self.terminal:
             if self.struck_count == 0:
                 # Nodes with zero struck count shouldn't have right and/or left nodes in non-cyclic shuffler.
                 if not cyclic and (self._right is not None or self._left is not None):
                     raise Exception("Unexpected right and/or left nodes at non-persisted node {}".format(self.key))
             else:
-                bit_manager: Final[BitManager] = self.bit_manager
+                bit_manager: Final[BitManager] = self.shuffler.bit_manager
                 bit: Final[int] = bit_manager.bit(self.bit_number)
 
                 right_size: int
                 left_size: int
 
                 if bit_manager.is_set(size, self.bit_number + 1):
                     # Size is the maximum possible and is split evenly between right and left nodes.
@@ -389,15 +184,15 @@
                 if right_size != size:
                     left = self.left
 
                     right_left_struck_count = right.struck_count + left.struck_count
                 else:
                     # Left node should be None if right node can handle this node.
                     if self._left is not None or \
-                            self.persistence_manager.restore_node_state(self.key - 1) is not None:
+                            self.shuffler.persistence_manager.restore_node_state(self.key - 1) is not None:
                         raise Exception("Unexpected left node at non-terminal node {}".format(self.key))
 
                     left = None
 
                     right_left_struck_count = right.struck_count
 
                 if self.struck_count != right_left_struck_count:
@@ -434,14 +229,49 @@
     The shuffler has two variants: non-cyclic and cyclic. The non-cyclic variant is the traditional Fisher-Yates
     shuffle, where the only requirement in the selection of the value for any unique index is that it not have been
     selected before. The cyclic variant is a lazy Sattolo algorithm, which requires that the value selected for any
     unique index be such that either it is not equal to the index for any previously generated index/value pair or that
     it link to the beginning of any open loop except its own.
     """
 
+    _TERMINAL_SIZE: Final[int] = 64
+    """
+    Terminal size (number of bits in qword).
+    """
+
+    _TERMINAL_SIZE_BITMASK: Final[int] = _TERMINAL_SIZE - 1
+    """
+    Terminal size bitmask.
+    """
+
+    _TERMINAL_SIZE_BIT_COUNT: Final[int] = _TERMINAL_SIZE_BITMASK.bit_count()
+    """
+    Terminal size bit count.
+    """
+
+    _TERMINAL_BIT_MANAGER: Final[BitManager] = BitManager(_TERMINAL_SIZE)
+    """
+    Bit manager for terminal struck bitmap manipulation.
+    """
+
+    _BIT_COUNT_BITMASK_2: Final[int] = 0x5555555555555555
+    """
+    Bitmask for 2 binary digits bit count (even bits).
+    """
+
+    _BIT_COUNT_BITMASK_4: Final[int] = 0x3333333333333333
+    """
+    Bitmask for 4 binary digits bit count (even 2-bit groups).
+    """
+
+    _BIT_COUNT_BITMASK_8: Final[int] = 0x0F0F0F0F0F0F0F0F
+    """
+    Bitmask for 8 binary digits bit count (even nibbles).
+    """
+
     def __init__(self, size: int, cyclic: bool, persistence_manager: Optional[PersistenceManager] = None):
         """
         Construct a shuffler.
 
         :param cyclic: If true, values are generated in a cyclic pattern.
 
         :param size: Size. Inputs and values range from 0 to size-1.
@@ -526,63 +356,180 @@
         Build the root based on the size.
         """
 
         resizing: Final[bool] = self._root is not None
 
         # If size is an exact power of two, subtracting 1 will force the bit length down by 1; round up to value for
         # full capacity terminal node if necessary.
-        size_bit_length: Final[int] = max((self.size - 1).bit_length(), _Node.TERMINAL_SIZE_BIT_COUNT)
+        size_bit_length: Final[int] = max((self.size - 1).bit_length(), Shuffler._TERMINAL_SIZE_BIT_COUNT)
 
         # New root must be created if not resizing (no root yet) or root bit number is changing.
         if not resizing or size_bit_length != self._root.bit_number + 1:
             # Bit manager is aligned with number of bits in root.
             self._bit_manager = BitManager(size_bit_length + 1)
 
             # Root key is 2^(size_bit_length+1)-1.
-            new_root: Final[_Node] = _Node(self.persistence_manager, self.bit_manager, self.bit_manager.all_bits,
-                                           size_bit_length - 1, not resizing)
+            new_root: Final[_Node] = _Node(self, self.bit_manager.all_bits, size_bit_length - 1, not resizing)
 
             if resizing:
                 # Copy struck count from old root.
                 root_struck_count: Final[int] = self._root.struck_count
 
                 # Nodes down the right from new root to above old root have to be properly constructed and persisted if
                 # struck count is non-zero.
                 if root_struck_count != 0:
                     update_node: Optional[_Node] = new_root
 
                     while update_node is not None:
                         update_node.struck_count = root_struck_count
 
-                        update_node.save_state()
+                        self.save_node_state(update_node)
 
                         # Update node is never terminal so there is always a right node.
                         update_node = update_node.right
 
                         # If right node has non-zero struck count, it's the old root and no further adjustments are
                         # required.
                         if update_node.struck_count != 0:
                             update_node = None
 
             self._root = new_root
 
         # Cache remaining size for performance.
         self._remaining_size = self.size - self._root.struck_count
 
+    def save_node_state(self, node: _Node):
+        """
+        Save node state to the persistence manager.
+
+        :param node: Node.
+        """
+
+        self.persistence_manager.save_node_state(node.key, NodeState(node.struck_count, node.struck_bitmap))
+
     def _next_value(self):
         """
         Generate the next value.
 
         :return: Next value, randomly selected from remaining unstruck entries.
         """
 
-        value: Final[int] = self._root.strike(self._random.randrange(0, self._remaining_size))
+        incremental_value: int = self._random.randrange(0, self._remaining_size)
 
         self._remaining_size -= 1
 
+        value: int = 0
+
+        node: Optional[_Node] = self._root
+
+        while node is not None:
+            pending_save_node: _Node = node
+
+            # One entry in current node or a descendant will be struck.
+            node.struck_count += 1
+
+            if not node.terminal:
+                right: _Node = node.right
+
+                # Normalize output to right node by adding number of struck entries in right node.
+                right_normalized_output: int = incremental_value + right.struck_count
+
+                # Index is in range of right node if current node's bit is clear.
+                if self.bit_manager.is_clear(right_normalized_output, node.bit_number):
+                    node = right
+                else:
+                    # Clear bit on incremental value and set bit on value to account for right normalized value.
+                    incremental_value = self.bit_manager.clear(right_normalized_output, node.bit_number)
+                    value = self.bit_manager.set(value, node.bit_number)
+
+                    node = node.left
+            else:
+                terminal_incremental_value_remaining: int = incremental_value
+                terminal_value: int
+
+                # These variables record the individual steps, except the last, of the bit count algorithm from Figure
+                # 5-2 of Hacker's Delight, 2nd edition, by Henry S. Warren, Jr., to count the bits in the unstruck
+                # bitmap.
+
+                # Each variable contains the count of the named number of bits repeating up to the size of a long
+                # integer (e.g., bitCount4 contains 16 counts of 4-bit sets).
+
+                # Need to find an unstruck bit, so invert the struck bitmap to begin.
+                bit_count_1: int = node.struck_bitmap ^ Shuffler._TERMINAL_BIT_MANAGER.all_bits
+                bit_count_2: int = bit_count_1 - (bit_count_1 >> 0x01 & Shuffler._BIT_COUNT_BITMASK_2)
+                bit_count_4: int = ((bit_count_2 & Shuffler._BIT_COUNT_BITMASK_4) +
+                                    (bit_count_2 >> 0x02 & Shuffler._BIT_COUNT_BITMASK_4))
+                bit_count_8: int = (bit_count_4 + (bit_count_4 >> 0x04)) & Shuffler._BIT_COUNT_BITMASK_8
+                bit_count_16: int = bit_count_8 + (bit_count_8 >> 0x08)
+                bit_count_32: int = bit_count_16 + (bit_count_16 >> 0x10)
+
+                # Starting with the broadest bit count, each block does the following:
+                #
+                #   1. Shifts the bit count to the right to accommodate the shift, stored in the terminal index,
+                #      determined by the previous steps (does not apply to the first block).
+                #   2. Extracts the right-most bit count and compares it to the incremental index remaining.
+                #   3. If less than or equal, the incremental index remaining is to the left, so:
+                #       a. subtracts the right-most bit count from the incremental index remaining; and
+                #       b. adds the number of bits considered (using bitwise "or" as all numbers are powers of 2) to the
+                #          terminal index (first block does straight assignment).
+                #
+                # Although a loop would yield cleaner code, the unrolled loop is faster.
+
+                right_bit_count: int
+
+                # 32-bit bit count; mask limits count to 0-32.
+                right_bit_count = bit_count_32 & 0x3F
+                if right_bit_count <= terminal_incremental_value_remaining:
+                    terminal_incremental_value_remaining -= right_bit_count
+                    terminal_value = 0x20
+                else:
+                    terminal_value = 0x00
+
+                # 16-bit bit count; mask limits count to 0-16.
+                right_bit_count = bit_count_16 >> terminal_value & 0x1F
+                if right_bit_count <= terminal_incremental_value_remaining:
+                    terminal_incremental_value_remaining -= right_bit_count
+                    terminal_value |= 0x10
+
+                # 8-bit bit count; mask limits count to 0-8.
+                right_bit_count = bit_count_8 >> terminal_value & 0x0F
+                if right_bit_count <= terminal_incremental_value_remaining:
+                    terminal_incremental_value_remaining -= right_bit_count
+                    terminal_value |= 0x08
+
+                # 4-bit bit count; mask limits count to 0-4.
+                right_bit_count = bit_count_4 >> terminal_value & 0x07
+                if right_bit_count <= terminal_incremental_value_remaining:
+                    terminal_incremental_value_remaining -= right_bit_count
+                    terminal_value |= 0x04
+
+                # 2-bit bit count; mask limits count to 0-2.
+                right_bit_count = bit_count_2 >> terminal_value & 0x03
+                if right_bit_count <= terminal_incremental_value_remaining:
+                    terminal_incremental_value_remaining -= right_bit_count
+                    terminal_value |= 0x02
+
+                # 1-bit bit count; mask limits count to 0-1.
+                right_bit_count = bit_count_1 >> terminal_value & 0x01
+                if right_bit_count <= terminal_incremental_value_remaining:
+                    terminal_incremental_value_remaining -= right_bit_count
+                    terminal_value |= 0x01
+
+                assert terminal_incremental_value_remaining == 0, "Terminal incremental output remaining is not zero"
+
+                # Set bit to mark entry as struck.
+                node.struck_bitmap = Shuffler._TERMINAL_BIT_MANAGER.set(node.struck_bitmap, terminal_value)
+
+                # Add terminal value to cumulative value.
+                value |= terminal_value
+
+                node = None
+
+            self.save_node_state(pending_save_node)
+
         return value
 
     def value_at(self, index: int) -> int:
         """
         Get the value at a given index. If the index is found in the persistence manager, the corresponding value is
         returned. Otherwise, a unique value is randomly generated and returned.
 
@@ -620,40 +567,75 @@
                     # Index is the end of an existing loop.
                     loop_start = ~value
                     not_loop_start = value
 
                     # Delete existing index/value pair.
                     self.persistence_manager.delete_index_value(index, value)
 
-                # Reserving the start of the loop prevents loop from closing on itself until the very end.
-                self._root.reserve(loop_start)
+                terminal_bit_number: Final[int] = loop_start & Shuffler._TERMINAL_SIZE_BITMASK
+
+                reserved_nodes: [_Node] = []
+
+                node: Optional[_Node] = self._root
+
+                while node is not None:
+                    pending_save_node: _Node = node
+
+                    reserved_nodes.append(node)
+
+                    # One entry in current node or a descendant is being reserved.
+                    node.struck_count += 1
+
+                    if not node.terminal:
+                        # Loop start is in range of right node if current node's bit is clear.
+                        node = node.right \
+                            if self.bit_manager.is_clear(loop_start, node.bit_number) else \
+                            node.left
+                    else:
+                        # Set bit to mark entry as struck.
+                        node.struck_bitmap = Shuffler._TERMINAL_BIT_MANAGER.set(node.struck_bitmap, terminal_bit_number)
+
+                        node = None
+
+                    self.save_node_state(pending_save_node)
 
                 # Account for reserve.
                 self._remaining_size -= 1
 
-                # Store reserve remaining size (faster than incrementing after unreserve).
-                reserve_remaining_size: Final[int] = self._remaining_size
+                # Store reserved remaining size (faster than incrementing after unreserve).
+                reserved_remaining_size: Final[int] = self._remaining_size
 
                 # Remaining size is zero if final loop is being closed.
                 if self._remaining_size != 0:
                     value = self._next_value()
 
                     # Persistence manager returns None if value is the end of its loop, otherwise value is the start of
                     # an existing loop that will be joined to this one.
                     loop_end: int = self._persistence_manager.index_of(~value)
                     if loop_end is None:
                         loop_end = value
 
                     # Join loop end to loop start with not bit value to indicate incompleteness.
                     self._persistence_manager.save_index_value(loop_end, not_loop_start)
 
-                    # Put the start of the loop back as a valid value.
-                    self._root.unreserve(loop_start)
+                    for reserved_node in reserved_nodes:
+                        # One entry in current node or a descendant is being unreserved.
+                        reserved_node.struck_count -= 1
+
+                        if reserved_node.terminal:
+                            # Clear bit to mark entry as unreserved.
+                            reserved_node.struck_bitmap = Shuffler._TERMINAL_BIT_MANAGER.clear(
+                                reserved_node.struck_bitmap, terminal_bit_number)
+
+                        if reserved_node.struck_count != 0:
+                            self.save_node_state(reserved_node)
+                        else:
+                            self.persistence_manager.delete_node_state(reserved_node.key)
 
-                    self._remaining_size = reserve_remaining_size
+                    self._remaining_size = reserved_remaining_size
                 else:
                     # Close the loop.
                     value = loop_start
 
         if randomized:
             # Store index/value pair.
             self._persistence_manager.save_index_value(index, value)
@@ -714,15 +696,15 @@
 
         for key in keys:
             if key == maximum_key:
                 raise Exception("Duplicate key {}".format(key))
 
             maximum_key = key
 
-        if minimum_key < _Node.TERMINAL_SIZE_BITMASK << 1 | 1:
+        if minimum_key < Shuffler._TERMINAL_SIZE_BITMASK << 1 | 1:
             raise Exception("Invalid minimum key {}".format(minimum_key))
 
         if maximum_key != minimum_key and maximum_key >= 1 << ((self.size - 1).bit_length() + 1):
             raise Exception("Invalid maximum key {}".format(maximum_key))
 
     class Iterator:
         """
```

### Comparing `lazy_fisher_yates_shuffler-1.0.0/PKG-INFO` & `lazy_fisher_yates_shuffler-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-fisher-yates-shuffler
-Version: 1.0.0
+Version: 1.0.1
 Summary: Lazy Fisher-Yates shuffler
 Home-page: https://github.com/KDean-Dolphin/Python-Shuffler
 License: Apache-2.0
 Author: Kevin Dean
 Author-email: Kevin.Dean@datadevelopment.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

