# Comparing `tmp/pystaleds-0.1.6.tar.gz` & `tmp/pystaleds-0.1.7.tar.gz`

## Comparing `pystaleds-0.1.6.tar` & `pystaleds-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 pystaleds-0.1.6/Cargo.toml
--rw-r--r--   0     1001      127     3526 2024-04-16 03:18:11.000000 pystaleds-0.1.6/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     1391 2024-04-16 03:18:11.000000 pystaleds-0.1.6/.github/workflows/linting.yml
--rw-r--r--   0     1001      127     2437 2024-04-16 03:18:11.000000 pystaleds-0.1.6/.github/workflows/tests.yml
--rw-r--r--   0     1001      127      686 2024-04-16 03:18:11.000000 pystaleds-0.1.6/.gitignore
--rw-r--r--   0     1001      127    27138 2024-04-16 03:18:16.000000 pystaleds-0.1.6/Cargo.lock
--rw-r--r--   0     1001      127     1062 2024-04-16 03:18:11.000000 pystaleds-0.1.6/LICENSE
--rw-r--r--   0     1001      127     5579 2024-04-16 03:18:11.000000 pystaleds-0.1.6/README.md
--rw-r--r--   0     1001      127     3084 2024-04-16 03:18:11.000000 pystaleds-0.1.6/src/ast_parsing.rs
--rw-r--r--   0     1001      127      324 2024-04-16 03:18:11.000000 pystaleds-0.1.6/src/debug.rs
--rw-r--r--   0     1001      127     9488 2024-04-16 03:18:11.000000 pystaleds-0.1.6/src/lexing.rs
--rw-r--r--   0     1001      127       81 2024-04-16 03:18:11.000000 pystaleds-0.1.6/src/lib.rs
--rw-r--r--   0     1001      127     8204 2024-04-16 03:18:11.000000 pystaleds-0.1.6/src/main.rs
--rw-r--r--   0     1001      127     7019 2024-04-16 03:18:11.000000 pystaleds-0.1.6/src/parsing.rs
--rw-r--r--   0     1001      127    27175 2024-04-16 03:18:11.000000 pystaleds-0.1.6/src/rules_checking.rs
--rw-r--r--   0     1001      127      335 2024-04-16 03:18:11.000000 pystaleds-0.1.6/test_folder/test.py
--rw-r--r--   0     1001      127      152 2024-04-16 03:18:11.000000 pystaleds-0.1.6/test_folder/test_cp.py
--rw-r--r--   0     1001      127      857 2024-04-16 03:18:11.000000 pystaleds-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6276 1970-01-01 00:00:00.000000 pystaleds-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 pystaleds-0.1.7/Cargo.toml
+-rw-r--r--   0     1001      127     3526 2024-04-19 01:11:59.000000 pystaleds-0.1.7/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     1391 2024-04-19 01:11:59.000000 pystaleds-0.1.7/.github/workflows/linting.yml
+-rw-r--r--   0     1001      127     2437 2024-04-19 01:11:59.000000 pystaleds-0.1.7/.github/workflows/tests.yml
+-rw-r--r--   0     1001      127      686 2024-04-19 01:11:59.000000 pystaleds-0.1.7/.gitignore
+-rw-r--r--   0     1001      127    27138 2024-04-19 01:11:59.000000 pystaleds-0.1.7/Cargo.lock
+-rw-r--r--   0     1001      127     1062 2024-04-19 01:11:59.000000 pystaleds-0.1.7/LICENSE
+-rw-r--r--   0     1001      127     5579 2024-04-19 01:11:59.000000 pystaleds-0.1.7/README.md
+-rw-r--r--   0     1001      127     3084 2024-04-19 01:11:59.000000 pystaleds-0.1.7/src/ast_parsing.rs
+-rw-r--r--   0     1001      127      324 2024-04-19 01:11:59.000000 pystaleds-0.1.7/src/debug.rs
+-rw-r--r--   0     1001      127    11034 2024-04-19 01:11:59.000000 pystaleds-0.1.7/src/lexing.rs
+-rw-r--r--   0     1001      127       81 2024-04-19 01:11:59.000000 pystaleds-0.1.7/src/lib.rs
+-rw-r--r--   0     1001      127     8825 2024-04-19 01:11:59.000000 pystaleds-0.1.7/src/main.rs
+-rw-r--r--   0     1001      127     8919 2024-04-19 01:11:59.000000 pystaleds-0.1.7/src/parsing.rs
+-rw-r--r--   0     1001      127    28322 2024-04-19 01:11:59.000000 pystaleds-0.1.7/src/rules_checking.rs
+-rw-r--r--   0     1001      127      335 2024-04-19 01:11:59.000000 pystaleds-0.1.7/test_folder/test.py
+-rw-r--r--   0     1001      127      152 2024-04-19 01:11:59.000000 pystaleds-0.1.7/test_folder/test_cp.py
+-rw-r--r--   0     1001      127      857 2024-04-19 01:11:59.000000 pystaleds-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6276 1970-01-01 00:00:00.000000 pystaleds-0.1.7/PKG-INFO
```

### Comparing `pystaleds-0.1.6/Cargo.toml` & `pystaleds-0.1.7/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pystaleds"
-version = "0.1.6"
+version = "0.1.7"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pystaleds"
 crate-type = ["lib"]
```

### Comparing `pystaleds-0.1.6/.github/workflows/CI.yml` & `pystaleds-0.1.7/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.6/.github/workflows/linting.yml` & `pystaleds-0.1.7/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.6/.github/workflows/tests.yml` & `pystaleds-0.1.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.6/.gitignore` & `pystaleds-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.6/Cargo.lock` & `pystaleds-0.1.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -450,15 +450,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
 name = "pystaleds"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
  "anyhow",
  "cc",
  "clap",
  "glob",
  "logos",
  "pyo3",
```

### Comparing `pystaleds-0.1.6/LICENSE` & `pystaleds-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.6/README.md` & `pystaleds-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.6/src/ast_parsing.rs` & `pystaleds-0.1.7/src/ast_parsing.rs`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.6/src/lexing.rs` & `pystaleds-0.1.7/src/lexing.rs`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 use logos::{Lexer, Logos, Source};
 
 use crate::ast_parsing::{FunctionInfo, FunctionLocation};
 
 pub fn get_next_function_info<'a, 'b>(
     lexer: &mut Lexer<'a, Token>,
     params: &'b mut Vec<(&'a str, Option<&'a str>)>,
+    skip_args_and_kwargs: bool,
 ) -> Option<FunctionInfo<'a, 'b>> {
     params.clear();
 
     while let Some(next) = lexer.next() {
         let Ok(Token::DefStart) = next else {
             continue;
         };
@@ -26,15 +27,18 @@
             let next = lexer.next();
             match next {
                 Some(Ok(Token::Colon)) => {
                     lexer.next();
 
                     let (typ, finished_on) = extract_possibly_parenthesized_content(lexer).ok()?;
 
-                    if param_name != "self" {
+                    if param_name != "self"
+                        && !(skip_args_and_kwargs
+                            && (param_name.starts_with('*') || param_name.starts_with("**")))
+                    {
                         params.push((param_name, Some(typ)));
                     }
 
                     match finished_on {
                         FinishedOn::Equals => {
                             lexer.next();
                             let (_, finished_on) =
@@ -51,24 +55,30 @@
                     }
                 }
                 Some(Ok(Token::Equals)) => {
                     lexer.next();
 
                     let (_, finished_on) = extract_possibly_parenthesized_content(lexer).ok()?;
 
-                    if param_name != "self" {
+                    if param_name != "self"
+                        && !(skip_args_and_kwargs
+                            && (param_name.starts_with('*') || param_name.starts_with("**")))
+                    {
                         params.push((param_name, None));
                     }
 
                     if let FinishedOn::ParClose = finished_on {
                         break;
                     }
                 }
                 _ => {
-                    if param_name != "self" {
+                    if param_name != "self"
+                        && !(skip_args_and_kwargs
+                            && (param_name.starts_with('*') || param_name.starts_with("**")))
+                    {
                         params.push((param_name, None));
                     }
                 }
             }
 
             current = lexer.next();
         }
@@ -217,22 +227,16 @@
 
     #[token(":")]
     Colon,
 
     #[token("=")]
     Equals,
 
-    #[token(r#"*args"#)]
-    Args,
-
-    #[token(r#"**kwargs"#)]
-    Kwargs,
-
     // Or regular expressions.
-    #[regex("[a-zA-Z0-9\'\"_|]+")]
+    #[regex("[a-zA-Z0-9\'\"_|*]+")]
     Text,
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
@@ -270,15 +274,15 @@
         let def = r#"def f(x, y: int=2, z=323):
     """Hello!""""#;
 
         let mut lex = Token::lexer(def);
 
         let mut params = Vec::new();
 
-        let function_info = get_next_function_info(&mut lex, &mut params).unwrap();
+        let function_info = get_next_function_info(&mut lex, &mut params, true).unwrap();
 
         assert_eq!(
             function_info.params,
             vec![("x", None), ("y", Some("int")), ("z", None)]
         );
 
         assert_eq!(function_info.function_name, FunctionLocation::Name("f"));
@@ -291,15 +295,15 @@
         let def = r#"def f(a, b: str = "wololo", c=323):
     """Hello!""""#;
 
         let mut lex = Token::lexer(def);
 
         let mut params = Vec::new();
 
-        get_next_function_info(&mut lex, &mut params);
+        get_next_function_info(&mut lex, &mut params, true);
 
         assert_eq!(params, vec![("a", None), ("b", Some("str")), ("c", None)]);
     }
 
     #[test]
     fn test_get_function_info3() {
         let def = r#"x=2
@@ -315,24 +319,88 @@
 
     "#;
 
         let mut lex = Token::lexer(def);
 
         let mut params = Vec::new();
 
-        get_next_function_info(&mut lex, &mut params);
+        get_next_function_info(&mut lex, &mut params, true);
 
         assert_eq!(params, vec![("a", None), ("b", None), ("c", None)]);
 
-        get_next_function_info(&mut lex, &mut params);
+        get_next_function_info(&mut lex, &mut params, true);
 
         assert_eq!(params, vec![("x", None), ("y", None)]);
     }
 
     #[test]
     fn test_extracting_parenthesized_content() {
         let mut lex = Token::lexer("[c{df}] , aklsdfjla");
         let (result, _) = extract_possibly_parenthesized_content(&mut lex).unwrap();
 
         assert_eq!(result, "[c{df}]")
     }
+
+    #[test]
+    fn test_args() {
+        let mut lex = Token::lexer(
+            r#"
+    def f(x, y, z, *args, a="oi"):
+        """Hello.
+
+
+
+
+
+        Nice spaces.
+
+
+        Arguments:
+            x:
+            y:
+            z:
+            """
+    "#,
+        );
+        let mut params = Vec::new();
+        get_next_function_info(&mut lex, &mut params, true).unwrap();
+
+        assert_eq!(
+            params,
+            vec![("x", None), ("y", None), ("z", None), ("a", None)]
+        );
+
+        let mut lex = Token::lexer(
+            r#"
+    def f(x, y, z, *args, a="oi"):
+        """Hello.
+
+
+
+
+
+        Nice spaces.
+
+
+        Arguments:
+            x:
+            y:
+            z:
+            """
+    "#,
+        );
+
+        let mut params = Vec::new();
+        get_next_function_info(&mut lex, &mut params, false).unwrap();
+
+        assert_eq!(
+            params,
+            vec![
+                ("x", None),
+                ("y", None),
+                ("z", None),
+                ("*args", None),
+                ("a", None)
+            ]
+        );
+    }
 }
```

### Comparing `pystaleds-0.1.6/src/main.rs` & `pystaleds-0.1.7/src/main.rs`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,19 @@
     forbid_no_args_in_docstring: bool,
 
     #[arg(long, default_value_t = false, alias = "nu")]
     /// Will consider an error for an arg in docstring to be untyped. Otherwise, only
     /// raises an error if the docstring's type and the signature's type are mismatched.
     forbid_untyped_docstrings: bool,
 
+    #[arg(long, default_value_t = false, alias = "ak")]
+    /// Will consider *args and **kwargs when checking the docstrings. If this flag is
+    /// not set, they are just completely ignored.
+    include_args_and_kwargs: bool,
+
     #[arg(short, long, default_value_t, value_enum)]
     /// Which parsing to use. Defaults to simple lexer, which is faster. Select
     /// `tree-sitter` in case you might be getting false positives/negatives.
     parser: CompliancyChecker,
 
     #[arg(short, long)]
     /// Runs over glob matches considering root to be the path specified in the command.
@@ -45,21 +50,23 @@
 
     #[arg(short, long, default_value_t, value_enum)]
     /// Determines the docstring style to consider for parsing.
     docstyle: DocstringStyle,
 }
 
 trait Compliancy {
+    #[allow(clippy::too_many_arguments)]
     fn is_file_compliant(
         &self,
         path: &Path,
         break_on_empty_line: bool,
         forbid_no_docstring: bool,
         forbid_no_args_in_docstring: bool,
         forbid_untyped_docstrings: bool,
+        args_and_kwargs: bool,
         docstyle: DocstringStyle,
     ) -> Result<bool>;
 }
 
 #[derive(Default, Clone, Copy, ValueEnum)]
 enum CompliancyChecker {
     TreeSitter,
@@ -72,31 +79,34 @@
     fn is_file_compliant(
         &self,
         path: &Path,
         break_on_empty_line: bool,
         forbid_no_docstring: bool,
         forbid_no_args_in_docstring: bool,
         forbid_untyped_docstrings: bool,
+        args_and_kwargs: bool,
         docstyle: DocstringStyle,
     ) -> Result<bool> {
         match self {
             CompliancyChecker::Lexer => is_file_compliant_lexing(
                 path,
                 break_on_empty_line,
                 forbid_no_docstring,
                 forbid_no_args_in_docstring,
                 forbid_untyped_docstrings,
+                args_and_kwargs,
                 docstyle,
             ),
             CompliancyChecker::TreeSitter => is_file_compliant_tree_sitter(
                 path,
                 break_on_empty_line,
                 forbid_no_docstring,
                 forbid_no_args_in_docstring,
                 forbid_untyped_docstrings,
+                args_and_kwargs,
                 docstyle,
             ),
         }
     }
 }
 
 /// Determines if a file or folder is hidden, i.e. if it starts with '.'.
@@ -107,14 +117,15 @@
 }
 
 fn main() -> Result<()> {
     let (non_blocking, _guard) = tracing_appender::non_blocking(std::io::stdout());
 
     tracing_subscriber::fmt()
         .without_time()
+        .with_target(false)
         .with_writer(non_blocking)
         .init();
 
     let args = Args::parse();
 
     if let CompliancyChecker::TreeSitter = args.parser {
         rayon::ThreadPoolBuilder::new()
@@ -175,14 +186,15 @@
 
             if args.parser.is_file_compliant(
                 path,
                 args.break_on_empty_line,
                 args.forbid_no_docstring,
                 args.forbid_no_args_in_docstring,
                 args.forbid_untyped_docstrings,
+                args.include_args_and_kwargs,
                 args.docstyle,
             )? {
                 0
             } else {
                 1
             }
         };
@@ -205,14 +217,15 @@
     if entry.is_file() && entry.extension() == Some(&std::ffi::OsString::from("py")) {
         let Ok(success) = args.parser.is_file_compliant(
             entry,
             args.break_on_empty_line,
             args.forbid_no_docstring,
             args.forbid_no_args_in_docstring,
             args.forbid_untyped_docstrings,
+            args.include_args_and_kwargs,
             args.docstyle,
         ) else {
             return;
         };
 
         if !success {
             total_errors.fetch_add(1, std::sync::atomic::Ordering::Relaxed);
@@ -223,14 +236,15 @@
 /// Determines if a file is compliant to the specified rules.
 fn is_file_compliant_tree_sitter(
     path: &Path,
     break_on_empty_line: bool,
     forbid_no_docstring: bool,
     forbid_no_args_in_docstring: bool,
     forbid_untyped_docstrings: bool,
+    args_and_kwargs: bool,
     docstyle: DocstringStyle,
 ) -> Result<bool> {
     let mut parser = tree_sitter::Parser::new();
     parser.set_language(&tree_sitter_python::language())?;
 
     let contents = std::fs::read_to_string(path)?;
 
@@ -239,39 +253,42 @@
         &contents,
         None,
         Some(path),
         break_on_empty_line,
         !forbid_no_docstring,
         !forbid_no_args_in_docstring,
         !forbid_untyped_docstrings,
+        !args_and_kwargs,
         docstyle,
     );
 
     Ok(success)
 }
 
 /// Determines if a file is compliant to the specified rules.
 fn is_file_compliant_lexing(
     path: &Path,
     break_on_empty_line: bool,
     forbid_no_docstring: bool,
     forbid_no_args_in_docstring: bool,
     forbid_untyped_docstrings: bool,
+    args_and_kwargs: bool,
     docstyle: DocstringStyle,
 ) -> Result<bool> {
     let mut parser = tree_sitter::Parser::new();
     parser.set_language(&tree_sitter_python::language())?;
 
     let contents = std::fs::read_to_string(path)?;
 
     let success = respects_rules_through_lexing(
         &contents,
         Some(path),
         break_on_empty_line,
         !forbid_no_docstring,
         !forbid_no_args_in_docstring,
         !forbid_untyped_docstrings,
+        !args_and_kwargs,
         docstyle,
     );
 
     Ok(success)
 }
```

### Comparing `pystaleds-0.1.6/src/rules_checking.rs` & `pystaleds-0.1.7/src/rules_checking.rs`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     source_code: &str,
     old_tree: Option<&Tree>,
     path: Option<&Path>,
     break_on_empty_line: bool,
     succeed_if_no_docstring: bool,
     succeed_if_no_args_in_docstring: bool,
     succeed_if_docstrings_are_not_typed: bool,
+    skip_args_and_kwargs: bool,
     docstyle: DocstringStyle,
 ) -> bool {
     let tree = parser
         .parse(source_code, old_tree)
         .expect("parser should be ready to parse");
 
     let mut cursor = tree.walk();
@@ -65,14 +66,15 @@
             if !is_function_info_valid(
                 &info,
                 path,
                 break_on_empty_line,
                 succeed_if_no_docstring,
                 succeed_if_no_args_in_docstring,
                 succeed_if_docstrings_are_not_typed,
+                skip_args_and_kwargs,
                 docstyle,
             ) {
                 success = false;
             }
         }
     });
 
@@ -84,75 +86,86 @@
 pub fn respects_rules_through_lexing(
     source_code: &str,
     path: Option<&Path>,
     break_on_empty_line: bool,
     succeed_if_no_docstring: bool,
     succeed_if_no_args_in_docstring: bool,
     succeed_if_docstrings_are_not_typed: bool,
+    skip_args_and_kwargs: bool,
     docstyle: DocstringStyle,
 ) -> bool {
     let mut lexer = Lexer::new(source_code);
 
     let mut success = true;
     let mut params = Vec::with_capacity(8);
 
-    while let Some(info) = get_next_function_info(&mut lexer, &mut params) {
+    while let Some(info) = get_next_function_info(&mut lexer, &mut params, skip_args_and_kwargs) {
         if !is_function_info_valid(
             &info,
             path,
             break_on_empty_line,
             succeed_if_no_docstring,
             succeed_if_no_args_in_docstring,
             succeed_if_docstrings_are_not_typed,
+            skip_args_and_kwargs,
             docstyle,
         ) {
             success = false;
         }
     }
 
     success
 }
 
 /// Checks if a given function respects the specified rules.
+#[allow(clippy::too_many_arguments)]
 fn is_function_info_valid(
     info: &FunctionInfo,
     path: Option<&Path>,
     break_on_empty_line: bool,
     succeed_if_no_docstring: bool,
     succeed_if_no_args_in_docstring: bool,
     succeed_if_docstrings_are_not_typed: bool,
+    skip_args_and_kwargs: bool,
     docstyle: DocstringStyle,
 ) -> bool {
     let path = path.map_or("".to_string(), |x| x.to_string_lossy().to_string() + ": ");
 
     let Some(docstring) = info.docstring else {
         if !succeed_if_no_docstring {
             tracing::event!(
                 Level::ERROR,
-                "{}{}: Docstring missing",
+                "{}`{}`: Docstring missing",
                 path,
                 info.function_name
             );
         }
 
         return succeed_if_no_docstring;
     };
 
     let args_from_docstring = match docstyle {
-        DocstringStyle::Google => parse_google_docstring(docstring, break_on_empty_line),
-        DocstringStyle::Numpy => parse_numpy_docstring(docstring, break_on_empty_line),
-        DocstringStyle::AutoDetect => parse_google_docstring(docstring, break_on_empty_line)
-            .or(parse_numpy_docstring(docstring, break_on_empty_line)),
+        DocstringStyle::Google => {
+            parse_google_docstring(docstring, break_on_empty_line, skip_args_and_kwargs)
+        }
+        DocstringStyle::Numpy => {
+            parse_numpy_docstring(docstring, break_on_empty_line, skip_args_and_kwargs)
+        }
+        DocstringStyle::AutoDetect => {
+            parse_google_docstring(docstring, break_on_empty_line, skip_args_and_kwargs).or(
+                parse_numpy_docstring(docstring, break_on_empty_line, skip_args_and_kwargs),
+            )
+        }
     };
 
     let Some(args_from_docstring) = args_from_docstring else {
         if !succeed_if_no_args_in_docstring {
             tracing::event!(
                 Level::ERROR,
-                "{}{}: Args missing from docstring",
+                "{}`{}`: Args missing from docstring",
                 path,
                 info.function_name
             );
         }
 
         return succeed_if_no_args_in_docstring;
     };
@@ -169,15 +182,15 @@
         } else {
             false
         };
 
         if !is_valid {
             tracing::event!(
                 Level::ERROR,
-                "{}{}: Args from function: {:?}. Args from docstring: {:?}",
+                "{}`{}`: Args from function: {:?}. Args from docstring: {:?}",
                 path,
                 info.function_name,
                 info.params,
                 args_from_docstring,
             );
         }
 
@@ -227,24 +240,26 @@
         assert!(is_function_info_valid(
             &function_info,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::AutoDetect
         ));
 
         assert!(!is_function_info_valid(
             &function_info,
             None,
             false,
             false,
             true,
             true,
+            true,
             DocstringStyle::AutoDetect
         ));
     }
 
     #[test]
     #[traced_test]
     fn test_out_of_order() {
@@ -266,14 +281,15 @@
         assert!(!is_function_info_valid(
             &function_info,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google
         ));
 
         let function_info = FunctionInfo {
             params: &[("x", Some("int")), ("y", Some("str"))],
             docstring: Some(
                 r#"
@@ -291,14 +307,15 @@
         assert!(is_function_info_valid(
             &function_info,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google
         ));
 
         let function_info = FunctionInfo {
             params: &[("x", Some("int")), ("y", Some("str"))],
             docstring: Some(
                 r#"
@@ -319,14 +336,15 @@
         assert!(!is_function_info_valid(
             &function_info,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Numpy
         ));
 
         let function_info = FunctionInfo {
             params: &[("x", Some("int")), ("y", Some("str"))],
             docstring: Some(
                 r#"
@@ -351,14 +369,15 @@
         assert!(is_function_info_valid(
             &function_info,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Numpy
         ));
     }
 
     #[test]
     #[traced_test]
     fn test_check_function_info() {
@@ -383,24 +402,26 @@
         assert!(is_function_info_valid(
             &function_info,
             None,
             false,
             false,
             false,
             true,
+            true,
             DocstringStyle::Google
         ));
 
         assert!(is_function_info_valid(
             &function_info,
             None,
             false,
             false,
             false,
             true,
+            true,
             DocstringStyle::AutoDetect
         ));
     }
 
     #[test]
     #[traced_test]
     fn ignore_edge_case() {
@@ -426,14 +447,15 @@
         assert!(is_function_info_valid(
             &function_info,
             None,
             false,
             false,
             false,
             true,
+            true,
             DocstringStyle::Google
         ));
     }
 
     #[test]
     #[traced_test]
     fn test_more_and_less_args() {
@@ -455,24 +477,26 @@
             source_code,
             None,
             None,
             false,
             true,
             true,
             true,
+            false,
             DocstringStyle::Google,
         ));
 
         assert!(respects_rules_through_lexing(
             source_code,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google,
         ));
 
         let source_code = r#"def sub(x, y):
     """This is a multi-line docstring.
 
     And this is the rest.
@@ -487,24 +511,26 @@
             source_code,
             None,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google,
         ));
 
         assert!(!respects_rules_through_lexing(
             source_code,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google,
         ));
 
         let source_code = r#"def sub(x, y):
     """This is a multi-line docstring.
 
     And this is the rest.
@@ -521,24 +547,26 @@
             source_code,
             None,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google,
         ));
 
         assert!(!respects_rules_through_lexing(
             source_code,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google,
         ));
     }
 
     #[test]
     #[traced_test]
     fn missing_args_docstring() {
@@ -568,24 +596,26 @@
             source_code,
             None,
             None,
             false,
             false,
             false,
             true,
+            true,
             DocstringStyle::Google,
         ));
 
         assert!(!respects_rules_through_lexing(
             source_code,
             None,
             false,
             false,
             false,
             true,
+            true,
             DocstringStyle::Google,
         ))
     }
 
     #[test]
     #[traced_test]
     fn test_file() {
@@ -615,24 +645,26 @@
             source_code,
             None,
             None,
             false,
             false,
             true,
             true,
+            true,
             DocstringStyle::Google,
         ));
 
         assert!(respects_rules_through_lexing(
             source_code,
             None,
             false,
             false,
             true,
             true,
+            true,
             DocstringStyle::Google,
         ));
     }
 
     #[test]
     #[traced_test]
     fn test_nesting() {
@@ -656,24 +688,26 @@
             source_code,
             None,
             None,
             false,
             true,
             true,
             false,
+            true,
             DocstringStyle::Google,
         ));
 
         assert!(!respects_rules_through_lexing(
             source_code,
             None,
             false,
             true,
             true,
             false,
+            true,
             DocstringStyle::Google,
         ));
 
         let source_code = r#"def add(x: int,y):
     """This is a docstring."""
     def sub(x: int, y: int):
         """This is a nested docstring.
@@ -691,24 +725,26 @@
             source_code,
             None,
             None,
             false,
             true,
             true,
             false,
+            true,
             DocstringStyle::Google,
         ));
 
         assert!(respects_rules_through_lexing(
             source_code,
             None,
             false,
             true,
             true,
             false,
+            true,
             DocstringStyle::Google,
         ));
     }
 
     #[test]
     fn test_from_path() {
         let mut parser = get_parser();
@@ -721,24 +757,26 @@
             &source_code,
             None,
             Some(&path),
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google
         ));
 
         assert!(respects_rules_through_lexing(
             &source_code,
             Some(&path),
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google
         ));
 
         let path = std::path::PathBuf::from("test_folder/test_cp.py");
         let source_code = std::fs::read_to_string("test_folder/test_cp.py").unwrap();
 
         assert!(!respects_rules(
@@ -746,24 +784,26 @@
             &source_code,
             None,
             Some(&path),
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google
         ));
 
         assert!(!respects_rules_through_lexing(
             &source_code,
             Some(&path),
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google
         ));
     }
 
     #[test]
     fn test_untyped_default_param() {
         let mut parser = get_parser();
@@ -786,24 +826,26 @@
             source_code,
             None,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google
         ));
 
         assert!(respects_rules_through_lexing(
             source_code,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google
         ));
     }
 
     #[test]
     fn test_break_on_new_line() {
         let mut parser = get_parser();
@@ -826,46 +868,50 @@
             source_code,
             None,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google
         ));
 
         assert!(!respects_rules_through_lexing(
             source_code,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google
         ));
 
         assert!(respects_rules(
             &mut parser,
             source_code,
             None,
             None,
             true,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google
         ));
 
         assert!(respects_rules_through_lexing(
             source_code,
             None,
             true,
             true,
             true,
             true,
+            true,
             DocstringStyle::Google
         ));
 
         let source_code = r#"def f(a, x=2):  # Comment to try and screw up the lexer.
     """
     Hey.
 
@@ -886,46 +932,50 @@
             source_code,
             None,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Numpy
         ));
 
         assert!(!respects_rules_through_lexing(
             source_code,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::Numpy
         ));
 
         assert!(respects_rules(
             &mut parser,
             source_code,
             None,
             None,
             true,
             true,
             true,
             true,
+            true,
             DocstringStyle::Numpy
         ));
 
         assert!(respects_rules_through_lexing(
             source_code,
             None,
             true,
             true,
             true,
             true,
+            true,
             DocstringStyle::Numpy
         ));
     }
 
     #[test]
     fn test_real_code() {
         let mut parser = get_parser();
@@ -1055,24 +1105,26 @@
             source_code,
             None,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::AutoDetect
         ));
 
         assert!(respects_rules_through_lexing(
             source_code,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::AutoDetect
         ));
     }
 
     #[test]
     fn test_real_code2() {
         let mut parser = get_parser();
@@ -1108,21 +1160,23 @@
             source_code,
             None,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::AutoDetect
         ));
 
         assert!(!respects_rules_through_lexing(
             source_code,
             None,
             false,
             true,
             true,
             true,
+            true,
             DocstringStyle::AutoDetect
         ));
     }
 }
```

### Comparing `pystaleds-0.1.6/pyproject.toml` & `pystaleds-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.6/PKG-INFO` & `pystaleds-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pystaleds
-Version: 0.1.6
+Version: 0.1.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Documentation
 License-File: LICENSE
 Summary: CLI tool for checking stale docstrings.
 Keywords: rust,docstrings,pre-commit,cli,tool,testing,ci
```

