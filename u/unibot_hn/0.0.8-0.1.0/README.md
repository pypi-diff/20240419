# Comparing `tmp/unibot_hn-0.0.8.tar.gz` & `tmp/unibot_hn-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unibot_hn-0.0.8.tar", max compression
+gzip compressed data, was "unibot_hn-0.1.0.tar", max compression
```

## Comparing `unibot_hn-0.0.8.tar` & `unibot_hn-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1066 2024-03-22 14:48:34.861774 unibot_hn-0.0.8/LICENSE
--rw-r--r--   0        0        0       14 2024-03-23 15:51:40.067352 unibot_hn-0.0.8/README.md
--rw-r--r--   0        0        0      316 2024-03-26 05:14:26.565442 unibot_hn-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-03-22 14:55:21.004090 unibot_hn-0.0.8/unibot_hn/.DS_Store
--rw-r--r--   0        0        0      426 2024-02-26 08:00:27.894916 unibot_hn-0.0.8/unibot_hn/Misc.py
--rw-r--r--   0        0        0     3696 2024-02-26 08:00:27.898217 unibot_hn-0.0.8/unibot_hn/PID.py
--rw-r--r--   0        0        0        0 2024-03-23 16:05:04.761382 unibot_hn-0.0.8/unibot_hn/__init__.py
--rw-r--r--   0        0        0    22001 2024-02-26 09:57:26.859814 unibot_hn-0.0.8/unibot_hn/board.py
--rw-r--r--   0        0        0    19870 2024-03-23 16:05:42.533817 unibot_hn-0.0.8/unibot_hn/camera.py
--rw-r--r--   0        0        0    12089 2024-03-26 05:14:10.015607 unibot_hn-0.0.8/unibot_hn/config_function.py
--rw-r--r--   0        0        0     7104 2024-02-26 09:58:19.954440 unibot_hn-0.0.8/unibot_hn/img_processing.py
--rw-r--r--   0        0        0     1680 2024-03-01 15:34:18.533544 unibot_hn-0.0.8/unibot_hn/robot_config.py
--rw-r--r--   0        0        0      676 2024-03-01 15:44:13.270021 unibot_hn-0.0.8/unibot_hn/robot_param_init.txt
--rw-r--r--   0        0        0     7727 2024-03-24 05:09:46.277825 unibot_hn-0.0.8/unibot_hn/servo_config_function.py
--rw-r--r--   0        0        0    21130 2024-03-26 05:10:40.644892 unibot_hn-0.0.8/unibot_hn/unibot.py
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 unibot_hn-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-22 14:48:34.861774 unibot_hn-0.1.0/LICENSE
+-rw-r--r--   0        0        0       14 2024-03-23 15:51:40.067352 unibot_hn-0.1.0/README.md
+-rw-r--r--   0        0        0      319 2024-04-19 10:11:24.553482 unibot_hn-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      426 2024-02-26 08:00:27.894916 unibot_hn-0.1.0/unibot_hn/Misc.py
+-rw-r--r--   0        0        0     3696 2024-02-26 08:00:27.898217 unibot_hn-0.1.0/unibot_hn/PID.py
+-rw-r--r--   0        0        0        0 2024-03-23 16:05:04.761382 unibot_hn-0.1.0/unibot_hn/__init__.py
+-rw-r--r--   0        0        0    22001 2024-02-26 09:57:26.859814 unibot_hn-0.1.0/unibot_hn/board.py
+-rw-r--r--   0        0        0    36032 2024-04-19 11:15:52.560156 unibot_hn-0.1.0/unibot_hn/camera.py
+-rw-r--r--   0        0        0     7104 2024-02-26 09:58:19.954440 unibot_hn-0.1.0/unibot_hn/img_processing.py
+-rw-r--r--   0        0        0     1680 2024-03-01 15:34:18.533544 unibot_hn-0.1.0/unibot_hn/robot_config.py
+-rw-r--r--   0        0        0      676 2024-03-01 15:44:13.270021 unibot_hn-0.1.0/unibot_hn/robot_param_init.txt
+-rw-r--r--   0        0        0     6301 2024-04-19 10:31:37.631075 unibot_hn-0.1.0/unibot_hn/setObjectColor.py
+-rw-r--r--   0        0        0     6296 2024-04-19 10:31:37.632369 unibot_hn-0.1.0/unibot_hn/setScreenObjectColor.py
+-rw-r--r--   0        0        0    23524 2024-04-19 11:15:19.100483 unibot_hn-0.1.0/unibot_hn/unibot.py
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 unibot_hn-0.1.0/PKG-INFO
```

### Comparing `unibot_hn-0.0.8/LICENSE` & `unibot_hn-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.8/unibot_hn/PID.py` & `unibot_hn-0.1.0/unibot_hn/PID.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.8/unibot_hn/board.py` & `unibot_hn-0.1.0/unibot_hn/board.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.8/unibot_hn/img_processing.py` & `unibot_hn-0.1.0/unibot_hn/img_processing.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.8/unibot_hn/robot_config.py` & `unibot_hn-0.1.0/unibot_hn/robot_config.py`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.8/unibot_hn/robot_param_init.txt` & `unibot_hn-0.1.0/unibot_hn/robot_param_init.txt`

 * *Files identical despite different names*

### Comparing `unibot_hn-0.0.8/unibot_hn/unibot.py` & `unibot_hn-0.1.0/unibot_hn/unibot.py`

 * *Files 7% similar despite different names*

```diff
@@ -473,36 +473,38 @@
                 valid, x1, y1, z1 = self.forward_kinematics(deg1, deg2, deg3, deg4)
                 v1, v2, v3, v4 = self.to_servo_value(deg1 + se1, deg2 + se2, deg3 + se3, deg4 + se4)
                 if abs(x1 - x) > 0.5 or abs(y1 - y) > 0.5 or abs(z1 - z) > 0.5:
                     pass
                 else:
                     self.board.bus_servo_set_position(t, [[1, int(v1)], [2, int(v2)], [3, int(v3)], [4, int(v4)]])
 
+
         except:
             print("角度解算失败")
+        time.sleep(t + 0.1)
 
     def angle_Kinematic(self, t, deg1, deg2, deg3, deg4):
         v1, v2, v3, v4 = self.to_servo_value(deg1, deg2, deg3, deg4)
         valid, x, y, z = self.forward_kinematics(deg1, deg2, deg3, deg4)
         # print('valid:{},x:{},y:{:f},z:{}'.format(valid,round(x,2),round(y,2),round(z,2)))
         self.board.bus_servo_set_position(t, [[1, int(v1)], [2, int(v2)], [3, int(v3)], [4, int(v4)]])
+        time.sleep(t + 0.1)
 
     def servo_enable_torque(self, enable):
         if enable:
             for _id in (1, 5):
                 self.board.bus_servo_enable_torque(_id, 1)
         else:
             for _id in (1, 5):
                 self.board.bus_servo_enable_torque(_id, 0)
 
-    def set_arm_servos_position(self, t,deg1, deg2, deg3, deg4):
+    def set_arm_servos_position(self, t, deg1, deg2, deg3, deg4):
         self.board.bus_servo_set_position(t, [[1, deg1], [2, deg2], [3, deg3], [4, deg4]])
 
 
-
 # 定义一个夹爪
 class Gripper:
     def __init__(self, board) -> None:
         self.board = board
 
     def action(self, duration, servo_degree, servo_id=1):
         """
@@ -557,15 +559,15 @@
     def follow_line(self, point_index):
         img = self.camera.get_frame()
         ls, lsc, img = self.camera.detect_vertical_black_line(img)
         self.camera.show_frame(img)
         try:
             return ls[point_index - 1][0]
         except:
-            return None
+            return -1
 
     # 旋转机器人寻找线
     def rotate_find_line(self, rotate_speed, endpointnum, point):
         self.robotic_arm.angle_Kinematic(0.3, 88, 40, -30, 90)
         self.chassis.move(0, 0, rotate_speed)
         img = self.camera.get_frame()
 
@@ -606,20 +608,81 @@
     def move_find_line(self, endpointnum=200):
         img = self.camera.get_frame()
         ls, lsc, img = self.camera.detect_vertical_black_line(img)
         self.camera.show_frame(img)
         if lsc[3] > endpointnum:
             return True
         else:
-            return False    
-        
-    def arm_to_holder(self,direction):
+            return False
+
+    def arm_to_holder(self, direction):
         if direction == 'left':
-            self.board.bus_servo_set_position(1, [[1, self.left_holder_servo_position['angle1']], [2, self.left_holder_servo_position['angle2']], [3, self.left_holder_servo_position['angle3']], [4, self.left_holder_servo_position['angle4']]])
-            
+            self.board.bus_servo_set_position(1, [[1, self.left_holder_servo_position['angle1']],
+                                                  [2, self.left_holder_servo_position['angle2']],
+                                                  [3, self.left_holder_servo_position['angle3']],
+                                                  [4, self.left_holder_servo_position['angle4']]])
+
         elif direction == 'right':
-            self.board.bus_servo_set_position(1, [[1, self.right_holder_servo_position['angle1']], [2, self.right_holder_servo_position['angle2']], [3, self.right_holder_servo_position['angle3']], [4, self.right_holder_servo_position['angle4']]])
+            self.board.bus_servo_set_position(1, [[1, self.right_holder_servo_position['angle1']],
+                                                  [2, self.right_holder_servo_position['angle2']],
+                                                  [3, self.right_holder_servo_position['angle3']],
+                                                  [4, self.right_holder_servo_position['angle4']]])
+
+    def align_object(self, p_x, p_y,error,min_x = 30,max_x = 290,min_y = 20,max_y = 260,target_area: int = 5000,speed=0):
+        color_flag = 3
+        cx = -1
+        cy = -1
+        for index in range(0, 3):
+            frame = self.camera.get_frame()
+        while color_flag == 3:
+            color_flag = self.camera.detect_object_color(5, target_area)
+            print(color_flag)
+        ans = 0
+        print("颜色：", color_flag)
+        while True:
+            cx, cy = self.camera.detect_object_center(color_flag, min_x,max_x,min_y,max_y ,target_area)
+            if cx != -1 and cy != -1:
+                #print(cx,cy)
+                error_x = cx - 160
+                error_y = cy - 120
+                px = error_x * p_x
+                py = error_y * p_y
 
+                if(abs(cx-160)<=error and abs(cy-120)<=error):
+                    ans+=1
+                else:
+                    if(abs(cx-160)<=8):
+                        px=0
+                    elif(px<0):
+                        px-=speed
+                    elif(px>0):
+                        px+=speed
+                    if(abs(cy-120)<=8):
+                        py=0
+                    elif(py<0):
+                        py-=speed
+                    elif(py>0):
+                        py+=speed
+                    ans=0
+                if(ans>=3):
+                    self.chassis.stop()
+                    break
+                print(px,py)
+                self.board.set_motor_speed([[1, px-py], [2, px+py], [3, -px-py], [4, -px+py]])
+
+
+        print("矫正结束")
+
+    def first_dected_object_rs(self):
+        target_color=self.camera.object_result('target_color')
+        target_shape=self.camera.object_result('target_shape')
+        now_color=self.camera.object_result('color')
+        now_shape=self.camera.object_result('shape')
+        print("当前检测结果和目标:",target_color,target_shape,now_color,now_shape)
+        if(target_color == now_color and target_shape == now_shape):
+            return True
+        else:
+            return False
 
 
 if __name__ == '__main__':
     my = Unibot()
```

### Comparing `unibot_hn-0.0.8/PKG-INFO` & `unibot_hn-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unibot_hn
-Version: 0.0.8
+Version: 0.1.0
 Summary: unibot_hn
 License: MIT
 Author: QuWan
 Requires-Python: >=3.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

