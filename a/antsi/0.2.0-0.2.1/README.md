# Comparing `tmp/antsi-0.2.0.tar.gz` & `tmp/antsi-0.2.1.tar.gz`

## Comparing `antsi-0.2.0.tar` & `antsi-0.2.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 antsi-0.2.0/Cargo.toml
--rw-r--r--   0     1001      127       22 2024-04-10 23:04:29.000000 antsi-0.2.0/.github/FUNDING.yml
--rw-r--r--   0     1001      127     4875 2024-04-10 23:04:29.000000 antsi-0.2.0/.github/workflows/distribution.yml
--rw-r--r--   0     1001      127      917 2024-04-10 23:04:29.000000 antsi-0.2.0/.github/workflows/lint.yml
--rw-r--r--   0     1001      127      685 2024-04-10 23:04:29.000000 antsi-0.2.0/.github/workflows/test.yml
--rw-r--r--   0     1001      127     5774 2024-04-10 23:04:29.000000 antsi-0.2.0/.gitignore
--rw-r--r--   0     1001      127      228 2024-04-10 23:04:29.000000 antsi-0.2.0/.yamllint.yml
--rw-r--r--   0     1001      127     1121 2024-04-10 23:04:29.000000 antsi-0.2.0/LICENSE.md
--rw-r--r--   0     1001      127     7995 2024-04-10 23:04:29.000000 antsi-0.2.0/README.md
--rw-r--r--   0     1001      127      402 2024-04-10 23:04:29.000000 antsi-0.2.0/antsi/__init__.py
--rw-r--r--   0     1001      127      158 2024-04-10 23:04:29.000000 antsi-0.2.0/antsi/_antsi.pyi
--rw-r--r--   0     1001      127        0 2024-04-10 23:04:29.000000 antsi-0.2.0/antsi/py.typed
--rw-r--r--   0     1001      127     7061 2024-04-10 23:04:29.000000 antsi-0.2.0/pdm.lock
--rw-r--r--   0     1001      127      107 2024-04-10 23:04:29.000000 antsi-0.2.0/renovate.json
--rw-r--r--   0     1001      127     2180 2024-04-10 23:04:29.000000 antsi-0.2.0/src/ast/color.rs
--rw-r--r--   0     1001      127     2071 2024-04-10 23:04:29.000000 antsi-0.2.0/src/ast/decoration.rs
--rw-r--r--   0     1001      127      271 2024-04-10 23:04:29.000000 antsi-0.2.0/src/ast/mod.rs
--rw-r--r--   0     1001      127    19008 2024-04-10 23:04:29.000000 antsi-0.2.0/src/ast/style.rs
--rw-r--r--   0     1001      127    14726 2024-04-10 23:04:29.000000 antsi-0.2.0/src/ast/token.rs
--rw-r--r--   0     1001      127    19103 2024-04-10 23:04:29.000000 antsi-0.2.0/src/color.rs
--rw-r--r--   0     1001      127     4554 2024-04-10 23:04:29.000000 antsi-0.2.0/src/error.rs
--rw-r--r--   0     1001      127     5386 2024-04-10 23:04:29.000000 antsi-0.2.0/src/escape.rs
--rw-r--r--   0     1001      127    11810 2024-04-10 23:04:29.000000 antsi-0.2.0/src/lexer.rs
--rw-r--r--   0     1001      127     4329 2024-04-10 23:04:29.000000 antsi-0.2.0/src/lib.rs
--rw-r--r--   0     1001      127     2401 2024-04-10 23:04:29.000000 antsi-0.2.0/src/macros.rs
--rw-r--r--   0     1001      127     8025 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/content.rs
--rw-r--r--   0     1001      127     4445 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/markup.rs
--rw-r--r--   0     1001      127      279 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__background_no_content.snap
--rw-r--r--   0     1001      127      347 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__decoration_multiple_styles_no_content.snap
--rw-r--r--   0     1001      127      319 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__decoration_single_style_no_content.snap
--rw-r--r--   0     1001      127      347 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__escaped_character_content.snap
--rw-r--r--   0     1001      127      278 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__foreground_no_content.snap
--rw-r--r--   0     1001      127      348 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__lowercase_alphabetic_content.snap
--rw-r--r--   0     1001      127      348 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__mixed_alphabetic_content.snap
--rw-r--r--   0     1001      127      671 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap
--rw-r--r--   0     1001      127      800 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap
--rw-r--r--   0     1001      127      735 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap
--rw-r--r--   0     1001      127      736 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap
--rw-r--r--   0     1001      127      348 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__numeric_content.snap
--rw-r--r--   0     1001      127      349 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__special_character_content.snap
--rw-r--r--   0     1001      127      348 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__uppercase_alphabetic_content.snap
--rw-r--r--   0     1001      127      394 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__empty_token.snap
--rw-r--r--   0     1001      127     2007 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap
--rw-r--r--   0     1001      127      907 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap
--rw-r--r--   0     1001      127      497 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_background.snap
--rw-r--r--   0     1001      127      496 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_foreground.snap
--rw-r--r--   0     1001      127      627 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap
--rw-r--r--   0     1001      127      562 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap
--rw-r--r--   0     1001      127      589 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap
--rw-r--r--   0     1001      127      694 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap
--rw-r--r--   0     1001      127      553 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap
--rw-r--r--   0     1001      127      563 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap
--rw-r--r--   0     1001      127    28591 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/style.rs
--rw-r--r--   0     1001      127    16007 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/text.rs
--rw-r--r--   0     1001      127    12470 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser.rs
--rw-r--r--   0     1001      127      314 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__lexer__tests__background_style_specifier.snap
--rw-r--r--   0     1001      127      310 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__lexer__tests__foreground_style_specifier.snap
--rw-r--r--   0     1001      127     3257 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__lexer__tests__many_tokens.snap
--rw-r--r--   0     1001      127      647 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__lexer__tests__mixed_whitespace_and_text.snap
--rw-r--r--   0     1001      127      490 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__lexer__tests__multiple_decoration_style_specifiers.snap
--rw-r--r--   0     1001      127      317 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__lexer__tests__single_decoration_style_specifier.snap
--rw-r--r--   0     1001      127      261 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__empty_token.snap
--rw-r--r--   0     1001      127     1567 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__kitchen_sink.snap
--rw-r--r--   0     1001      127      670 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__nested_token.snap
--rw-r--r--   0     1001      127      230 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_bad_escape_character@errors.snap
--rw-r--r--   0     1001      127      111 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_bad_escape_character@result.snap
--rw-r--r--   0     1001      127      242 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@errors.snap
--rw-r--r--   0     1001      127      355 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@result.snap
--rw-r--r--   0     1001      127      157 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_text.snap
--rw-r--r--   0     1001      127      231 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@errors.snap
--rw-r--r--   0     1001      127      107 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@result.snap
--rw-r--r--   0     1001      127      245 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@errors.snap
--rw-r--r--   0     1001      127      385 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@result.snap
--rw-r--r--   0     1001      127      235 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@errors.snap
--rw-r--r--   0     1001      127      109 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@result.snap
--rw-r--r--   0     1001      127      620 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap
--rw-r--r--   0     1001      127      112 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@result.snap
--rw-r--r--   0     1001      127      230 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@errors.snap
--rw-r--r--   0     1001      127      107 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@result.snap
--rw-r--r--   0     1001      127      614 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap
--rw-r--r--   0     1001      127      112 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@result.snap
--rw-r--r--   0     1001      127      502 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_plaintext@errors.snap
--rw-r--r--   0     1001      127      685 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_token@errors.snap
--rw-r--r--   0     1001      127      338 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_background.snap
--rw-r--r--   0     1001      127      336 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_foreground.snap
--rw-r--r--   0     1001      127      438 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_leading_and_trailing_content.snap
--rw-r--r--   0     1001      127      388 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_leading_content.snap
--rw-r--r--   0     1001      127      414 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_multiple_decorations.snap
--rw-r--r--   0     1001      127      502 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_multiple_styles.snap
--rw-r--r--   0     1001      127      379 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_single_decoration.snap
--rw-r--r--   0     1001      127      390 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_trailing_content.snap
--rw-r--r--   0     1001      127    15847 2024-04-10 23:04:29.000000 antsi-0.2.0/Cargo.lock
--rw-r--r--   0     1001      127     1056 2024-04-10 23:04:29.000000 antsi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8598 1970-01-01 00:00:00.000000 antsi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 antsi-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      127       22 2024-04-19 05:36:06.000000 antsi-0.2.1/.github/FUNDING.yml
+-rw-r--r--   0     1001      127     4875 2024-04-19 05:36:06.000000 antsi-0.2.1/.github/workflows/distribution.yml
+-rw-r--r--   0     1001      127      917 2024-04-19 05:36:06.000000 antsi-0.2.1/.github/workflows/lint.yml
+-rw-r--r--   0     1001      127      685 2024-04-19 05:36:06.000000 antsi-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0     1001      127     5774 2024-04-19 05:36:06.000000 antsi-0.2.1/.gitignore
+-rw-r--r--   0     1001      127      228 2024-04-19 05:36:06.000000 antsi-0.2.1/.yamllint.yml
+-rw-r--r--   0     1001      127     1121 2024-04-19 05:36:06.000000 antsi-0.2.1/LICENSE.md
+-rw-r--r--   0     1001      127     7995 2024-04-19 05:36:06.000000 antsi-0.2.1/README.md
+-rw-r--r--   0     1001      127      402 2024-04-19 05:36:06.000000 antsi-0.2.1/antsi/__init__.py
+-rw-r--r--   0     1001      127      206 2024-04-19 05:36:06.000000 antsi-0.2.1/antsi/_antsi.pyi
+-rw-r--r--   0     1001      127        0 2024-04-19 05:36:06.000000 antsi-0.2.1/antsi/py.typed
+-rw-r--r--   0     1001      127     7061 2024-04-19 05:36:06.000000 antsi-0.2.1/pdm.lock
+-rw-r--r--   0     1001      127      107 2024-04-19 05:36:06.000000 antsi-0.2.1/renovate.json
+-rw-r--r--   0     1001      127     2180 2024-04-19 05:36:06.000000 antsi-0.2.1/src/ast/color.rs
+-rw-r--r--   0     1001      127     2071 2024-04-19 05:36:06.000000 antsi-0.2.1/src/ast/decoration.rs
+-rw-r--r--   0     1001      127      271 2024-04-19 05:36:06.000000 antsi-0.2.1/src/ast/mod.rs
+-rw-r--r--   0     1001      127    19008 2024-04-19 05:36:06.000000 antsi-0.2.1/src/ast/style.rs
+-rw-r--r--   0     1001      127    14726 2024-04-19 05:36:06.000000 antsi-0.2.1/src/ast/token.rs
+-rw-r--r--   0     1001      127    21250 2024-04-19 05:36:06.000000 antsi-0.2.1/src/color.rs
+-rw-r--r--   0     1001      127     4554 2024-04-19 05:36:06.000000 antsi-0.2.1/src/error.rs
+-rw-r--r--   0     1001      127     5386 2024-04-19 05:36:06.000000 antsi-0.2.1/src/escape.rs
+-rw-r--r--   0     1001      127    11810 2024-04-19 05:36:06.000000 antsi-0.2.1/src/lexer.rs
+-rw-r--r--   0     1001      127     4449 2024-04-19 05:36:06.000000 antsi-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      127     2401 2024-04-19 05:36:06.000000 antsi-0.2.1/src/macros.rs
+-rw-r--r--   0     1001      127     8025 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/content.rs
+-rw-r--r--   0     1001      127     4445 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/markup.rs
+-rw-r--r--   0     1001      127      279 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__background_no_content.snap
+-rw-r--r--   0     1001      127      347 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__decoration_multiple_styles_no_content.snap
+-rw-r--r--   0     1001      127      319 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__decoration_single_style_no_content.snap
+-rw-r--r--   0     1001      127      347 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__escaped_character_content.snap
+-rw-r--r--   0     1001      127      278 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__foreground_no_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__lowercase_alphabetic_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__mixed_alphabetic_content.snap
+-rw-r--r--   0     1001      127      671 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap
+-rw-r--r--   0     1001      127      800 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap
+-rw-r--r--   0     1001      127      735 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap
+-rw-r--r--   0     1001      127      736 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__numeric_content.snap
+-rw-r--r--   0     1001      127      349 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__special_character_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__uppercase_alphabetic_content.snap
+-rw-r--r--   0     1001      127      394 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__empty_token.snap
+-rw-r--r--   0     1001      127     2007 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap
+-rw-r--r--   0     1001      127      907 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap
+-rw-r--r--   0     1001      127      497 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__token_with_background.snap
+-rw-r--r--   0     1001      127      496 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__token_with_foreground.snap
+-rw-r--r--   0     1001      127      627 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap
+-rw-r--r--   0     1001      127      562 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap
+-rw-r--r--   0     1001      127      589 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap
+-rw-r--r--   0     1001      127      694 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap
+-rw-r--r--   0     1001      127      553 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap
+-rw-r--r--   0     1001      127      563 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap
+-rw-r--r--   0     1001      127    28591 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/style.rs
+-rw-r--r--   0     1001      127    16007 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser/text.rs
+-rw-r--r--   0     1001      127    12470 2024-04-19 05:36:06.000000 antsi-0.2.1/src/parser.rs
+-rw-r--r--   0     1001      127      314 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__lexer__tests__background_style_specifier.snap
+-rw-r--r--   0     1001      127      310 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__lexer__tests__foreground_style_specifier.snap
+-rw-r--r--   0     1001      127     3257 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__lexer__tests__many_tokens.snap
+-rw-r--r--   0     1001      127      647 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__lexer__tests__mixed_whitespace_and_text.snap
+-rw-r--r--   0     1001      127      490 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__lexer__tests__multiple_decoration_style_specifiers.snap
+-rw-r--r--   0     1001      127      317 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__lexer__tests__single_decoration_style_specifier.snap
+-rw-r--r--   0     1001      127      261 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__empty_token.snap
+-rw-r--r--   0     1001      127     1567 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__kitchen_sink.snap
+-rw-r--r--   0     1001      127      670 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__nested_token.snap
+-rw-r--r--   0     1001      127      230 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_bad_escape_character@errors.snap
+-rw-r--r--   0     1001      127      111 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_bad_escape_character@result.snap
+-rw-r--r--   0     1001      127      242 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@errors.snap
+-rw-r--r--   0     1001      127      355 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@result.snap
+-rw-r--r--   0     1001      127      157 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_text.snap
+-rw-r--r--   0     1001      127      231 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@errors.snap
+-rw-r--r--   0     1001      127      107 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@result.snap
+-rw-r--r--   0     1001      127      245 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@errors.snap
+-rw-r--r--   0     1001      127      385 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@result.snap
+-rw-r--r--   0     1001      127      235 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@errors.snap
+-rw-r--r--   0     1001      127      109 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@result.snap
+-rw-r--r--   0     1001      127      620 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap
+-rw-r--r--   0     1001      127      112 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@result.snap
+-rw-r--r--   0     1001      127      230 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@errors.snap
+-rw-r--r--   0     1001      127      107 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@result.snap
+-rw-r--r--   0     1001      127      614 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap
+-rw-r--r--   0     1001      127      112 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@result.snap
+-rw-r--r--   0     1001      127      502 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_plaintext@errors.snap
+-rw-r--r--   0     1001      127      685 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_token@errors.snap
+-rw-r--r--   0     1001      127      338 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__token_with_background.snap
+-rw-r--r--   0     1001      127      336 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__token_with_foreground.snap
+-rw-r--r--   0     1001      127      438 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__token_with_leading_and_trailing_content.snap
+-rw-r--r--   0     1001      127      388 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__token_with_leading_content.snap
+-rw-r--r--   0     1001      127      414 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__token_with_multiple_decorations.snap
+-rw-r--r--   0     1001      127      502 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__token_with_multiple_styles.snap
+-rw-r--r--   0     1001      127      379 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__token_with_single_decoration.snap
+-rw-r--r--   0     1001      127      390 2024-04-19 05:36:06.000000 antsi-0.2.1/src/snapshots/antsi__parser__tests__token_with_trailing_content.snap
+-rw-r--r--   0     1001      127    15847 2024-04-19 05:36:06.000000 antsi-0.2.1/Cargo.lock
+-rw-r--r--   0     1001      127     1056 2024-04-19 05:36:06.000000 antsi-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8598 1970-01-01 00:00:00.000000 antsi-0.2.1/PKG-INFO
```

### Comparing `antsi-0.2.0/Cargo.toml` & `antsi-0.2.1/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "antsi"
-version = "0.2.0"
+version = "0.2.1"
 edition = "2021"
 description = "A quick and user-friendly way to style your text using ANSI codes"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "antsi"
 crate-type = ["cdylib"]
```

### Comparing `antsi-0.2.0/.github/workflows/distribution.yml` & `antsi-0.2.1/.github/workflows/distribution.yml`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/.github/workflows/lint.yml` & `antsi-0.2.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/.github/workflows/test.yml` & `antsi-0.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/.gitignore` & `antsi-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/LICENSE.md` & `antsi-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/README.md` & `antsi-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/pdm.lock` & `antsi-0.2.1/pdm.lock`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/ast/color.rs` & `antsi-0.2.1/src/ast/color.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/ast/decoration.rs` & `antsi-0.2.1/src/ast/decoration.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/ast/style.rs` & `antsi-0.2.1/src/ast/style.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/ast/token.rs` & `antsi-0.2.1/src/ast/token.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/color.rs` & `antsi-0.2.1/src/color.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,38 @@
 use crate::{
     ast::{CurrentStyle, Token},
     error::Error,
     parser::Parser,
 };
 
-pub fn colorize(input: &str) -> Result<String, Vec<Error>> {
+#[derive(Clone, Copy, Debug)]
+pub struct Options {
+    pub supports_color: bool,
+}
+
+impl Default for Options {
+    fn default() -> Self {
+        Self {
+            supports_color: true,
+        }
+    }
+}
+
+pub fn colorize(input: &str, options: Options) -> Result<String, Vec<Error>> {
     let (tokens, errors) = Parser::new(input).parse();
     if !errors.is_empty() {
         return Err(errors);
     }
 
     let mut result = String::with_capacity(input.len());
-    convert_tokens(&mut result, CurrentStyle::default(), &tokens);
+    if options.supports_color {
+        convert_tokens(&mut result, CurrentStyle::default(), &tokens);
+    } else {
+        convert_tokens_no_color(&mut result, &tokens);
+    }
 
     result.shrink_to_fit();
     Ok(result)
 }
 
 /// Convert the tokens into the resulting string
 fn convert_tokens(output: &mut String, parent_style: CurrentStyle, tokens: &[Token]) {
@@ -31,17 +48,33 @@
                 convert_tokens(output, parent_style.extend(style), content);
                 style.reset(&parent_style, output);
             }
         }
     }
 }
 
+/// Convert the tokens into the resulting string without applying styles
+fn convert_tokens_no_color(output: &mut String, tokens: &[Token]) {
+    for token in tokens {
+        match token {
+            Token::Content(content) => output.push_str(content),
+            Token::Styled { content, .. } => {
+                if content.is_empty() {
+                    continue;
+                }
+
+                convert_tokens_no_color(output, content);
+            }
+        }
+    }
+}
+
 #[cfg(test)]
 mod tests {
-    use super::colorize;
+    use super::{colorize, Options};
     use crate::ast::{Style, Token};
 
     fn convert_tokens(parent_style: Option<Style>, tokens: &[Token]) -> String {
         let mut result = String::new();
         super::convert_tokens(&mut result, parent_style.unwrap_or_default().into(), tokens);
         result
     }
@@ -412,167 +445,198 @@
             }],
         );
         assert_eq!(result, "\x1b[44mred \x1b[31mblue\x1b[39m red\x1b[49m");
     }
 
     #[test]
     fn colorize_empty_source() {
-        let result = colorize("").unwrap();
+        let result = colorize("", Options::default()).unwrap();
         assert_eq!(result, "");
     }
 
     #[test]
     fn colorize_source_with_no_styled_content() {
-        let result = colorize("unstyled content").unwrap();
+        let result = colorize("unstyled content", Options::default()).unwrap();
         assert_eq!(result, "unstyled content");
     }
 
     #[test]
     fn colorize_styled_content_spanning_entire_source() {
-        let result = colorize("[fg:black](content)").unwrap();
+        let result = colorize("[fg:black](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[30mcontent\x1b[39m");
     }
 
     #[test]
     fn colorize_styled_content_starting_at_beginning() {
-        let result = colorize("[fg:black](content) unstyled").unwrap();
+        let result = colorize("[fg:black](content) unstyled", Options::default()).unwrap();
         assert_eq!(result, "\x1b[30mcontent\x1b[39m unstyled");
     }
 
     #[test]
     fn colorize_styled_content_starting_in_middle() {
-        let result = colorize("leading [fg:black](content) trailing").unwrap();
+        let result = colorize("leading [fg:black](content) trailing", Options::default()).unwrap();
         assert_eq!(result, "leading \x1b[30mcontent\x1b[39m trailing");
     }
 
     #[test]
     fn colorize_styled_content_starting_at_end() {
-        let result = colorize("leading [fg:black](content)").unwrap();
+        let result = colorize("leading [fg:black](content)", Options::default()).unwrap();
         assert_eq!(result, "leading \x1b[30mcontent\x1b[39m");
     }
 
     #[test]
     fn colorize_styled_with_foreground() {
-        let result = colorize("[fg:red](content)").unwrap();
+        let result = colorize("[fg:red](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[31mcontent\x1b[39m");
     }
 
     #[test]
     fn colorize_styled_with_background() {
-        let result = colorize("[bg:red](content)").unwrap();
+        let result = colorize("[bg:red](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[41mcontent\x1b[49m");
     }
 
     #[test]
     fn colorize_styled_with_decoration() {
-        let result = colorize("[deco:bold](content)").unwrap();
+        let result = colorize("[deco:bold](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[1mcontent\x1b[22m");
     }
 
     #[test]
     fn colorize_styled_with_foreground_and_background() {
-        let result = colorize("[fg:red;bg:white](content)").unwrap();
+        let result = colorize("[fg:red;bg:white](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[31;47mcontent\x1b[39;49m");
     }
 
     #[test]
     fn colorize_styled_with_foreground_and_decoration() {
-        let result = colorize("[fg:red;deco:bold](content)").unwrap();
+        let result = colorize("[fg:red;deco:bold](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[31;1mcontent\x1b[39;22m");
     }
 
     #[test]
     fn colorize_styled_with_decoration_and_background() {
-        let result = colorize("[deco:bold;bg:white](content)").unwrap();
+        let result = colorize("[deco:bold;bg:white](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[47;1mcontent\x1b[49;22m");
     }
 
     #[test]
     fn colorize_styled_with_background_and_foreground() {
-        let result = colorize("[bg:white;fg:red](content)").unwrap();
+        let result = colorize("[bg:white;fg:red](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[31;47mcontent\x1b[39;49m");
     }
 
     #[test]
     fn colorize_styled_with_decoration_and_foreground() {
-        let result = colorize("[deco:bold;fg:red](content)").unwrap();
+        let result = colorize("[deco:bold;fg:red](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[31;1mcontent\x1b[39;22m");
     }
 
     #[test]
     fn colorize_styled_with_background_and_decoration() {
-        let result = colorize("[bg:white;deco:bold](content)").unwrap();
+        let result = colorize("[bg:white;deco:bold](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[47;1mcontent\x1b[49;22m");
     }
 
     #[test]
     fn colorize_styled_with_foreground_background_and_decoration() {
-        let result = colorize("[fg:red;bg:white;deco:bold](content)").unwrap();
+        let result = colorize("[fg:red;bg:white;deco:bold](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[31;47;1mcontent\x1b[39;49;22m");
     }
 
     #[test]
     fn colorize_styled_with_foreground_decoration_and_background() {
-        let result = colorize("[fg:red;deco:bold;bg:white](content)").unwrap();
+        let result = colorize("[fg:red;deco:bold;bg:white](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[31;47;1mcontent\x1b[39;49;22m");
     }
 
     #[test]
     fn colorize_styled_with_background_foreground_and_decoration() {
-        let result = colorize("[bg:white;fg:red;deco:bold](content)").unwrap();
+        let result = colorize("[bg:white;fg:red;deco:bold](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[31;47;1mcontent\x1b[39;49;22m");
     }
 
     #[test]
     fn colorize_styled_with_background_decoration_and_foreground() {
-        let result = colorize("[bg:white;deco:bold;fg:red](content)").unwrap();
+        let result = colorize("[bg:white;deco:bold;fg:red](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[31;47;1mcontent\x1b[39;49;22m");
     }
 
     #[test]
     fn colorize_styled_with_decoration_foreground_and_background() {
-        let result = colorize("[deco:bold;fg:red;bg:white](content)").unwrap();
+        let result = colorize("[deco:bold;fg:red;bg:white](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[31;47;1mcontent\x1b[39;49;22m");
     }
 
     #[test]
     fn colorize_styled_with_decoration_background_and_foreground() {
-        let result = colorize("[deco:bold;bg:white;fg:red](content)").unwrap();
+        let result = colorize("[deco:bold;bg:white;fg:red](content)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[31;47;1mcontent\x1b[39;49;22m");
     }
 
     #[test]
     fn colorize_token_not_produced_for_content_with_zero_length() {
-        let result = colorize("[fg:red]()").unwrap();
+        let result = colorize("[fg:red]()", Options::default()).unwrap();
         assert_eq!(result, "");
     }
 
     #[test]
     fn colorize_two_spans_of_styled_text_back_to_back() {
-        let result = colorize("[fg:red](first)[fg:blue](second)").unwrap();
+        let result = colorize("[fg:red](first)[fg:blue](second)", Options::default()).unwrap();
         assert_eq!(result, "\x1b[31mfirst\x1b[39m\x1b[34msecond\x1b[39m");
     }
 
     #[test]
     fn colorize_spans_of_styled_text_interleaved_with_unstyled_text() {
-        let result =
-            colorize("leading [fg:red](styled one) middle [fg:blue](styled two) trailing").unwrap();
+        let result = colorize(
+            "leading [fg:red](styled one) middle [fg:blue](styled two) trailing",
+            Options::default(),
+        )
+        .unwrap();
         assert_eq!(
             result,
             "leading \x1b[31mstyled one\x1b[39m middle \x1b[34mstyled two\x1b[39m trailing"
         );
     }
 
     #[test]
     fn colorize_when_style_tags_are_repeated_the_last_occurrence_takes_precedence() {
-        let result =
-            colorize("[fg:black;bg:white;deco:bold;fg:white;bg:black;deco:faint](content)")
-                .unwrap();
+        let result = colorize(
+            "[fg:black;bg:white;deco:bold;fg:white;bg:black;deco:faint](content)",
+            Options::default(),
+        )
+        .unwrap();
         assert_eq!(result, "\x1b[37;40;2mcontent\x1b[39;49;22m");
     }
 
     #[test]
     fn colorize_nested_styled_spans_produce_multiple_styled_tokens() {
-        let result = colorize("user: [deco:bold](hi [fg:red](there)!)").unwrap();
+        let result =
+            colorize("user: [deco:bold](hi [fg:red](there)!)", Options::default()).unwrap();
         assert_eq!(result, "user: \x1b[1mhi \x1b[31mthere\x1b[39m!\x1b[22m");
     }
+
+    #[test]
+    fn colorize_kitchen_sink() {
+        let result = colorize(
+            "leading [fg:red](one [bg:blue](two [deco:dim](three) two) one) trailing",
+            Options::default(),
+        )
+        .unwrap();
+        assert_eq!(
+            result,
+            "leading \x1b[31mone \x1b[44mtwo \x1b[2mthree\x1b[22m two\x1b[49m one\x1b[39m trailing"
+        );
+    }
+
+    #[test]
+    fn colorize_kitchen_sink_color_disabled() {
+        let result = colorize(
+            "leading [fg:red](one [bg:blue](two [deco:dim](three) two) one) trailing",
+            Options {
+                supports_color: false,
+            },
+        )
+        .unwrap();
+        assert_eq!(result, "leading one two three two one trailing");
+    }
 }
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_13ce0_3q_/tmpqandmifc_TarContainer/0/19.rs", line 579, column 0: CDATA terminal not found*

```diff
@@ -1,13 +1,21 @@
-use crate::{ ast::{CurrentStyle, Token}, error::Error, parser::Parser, }; pub
-fn colorize(input: &str) -> Result
+use crate::{ ast::{CurrentStyle, Token}, error::Error, parser::Parser, }; #
+[derive(Clone, Copy, Debug)] pub struct Options { pub supports_color: bool, }
+impl Default for Options { fn default() -> Self { Self { supports_color: true,
+} } } pub fn colorize(input: &str, options: Options) -> Result
  Vec> { let (tokens, errors) = Parser::new(input).parse(); if !errors.is_empty
 () { return Err(errors); } let mut result = String::with_capacity(input.len());
-convert_tokens(&mut result, CurrentStyle::default(), &tokens);
+if options.supports_color { convert_tokens(&mut result, CurrentStyle::default
+(), &tokens); } else { convert_tokens_no_color(&mut result, &tokens); }
 result.shrink_to_fit(); Ok(result) } /// Convert the tokens into the resulting
 string fn convert_tokens(output: &mut String, parent_style: CurrentStyle,
 tokens: &[Token]) { for token in tokens { match token { Token::Content(content)
 => output.push_str(content), Token::Styled { content, style } => { if
 content.is_empty() { continue; } style.apply(&parent_style, output);
 convert_tokens(output, parent_style.extend(style), content); style.reset
-(&parent_style, output); } } } } #[cfg(test)] mod tests { use super::colorize;
-use crate::ast::{Style, Token}; fn convert_tokens(parent_style: Option
+(&parent_style, output); } } } } /// Convert the tokens into the resulting
+string without applying styles fn convert_tokens_no_color(output: &mut String,
+tokens: &[Token]) { for token in tokens { match token { Token::Content(content)
+=> output.push_str(content), Token::Styled { content, .. } => { if
+content.is_empty() { continue; } convert_tokens_no_color(output, content); } }
+} } #[cfg(test)] mod tests { use super::{colorize, Options}; use crate::ast::
+{Style, Token}; fn convert_tokens(parent_style: Option
```

### Comparing `antsi-0.2.0/src/error.rs` & `antsi-0.2.1/src/error.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/escape.rs` & `antsi-0.2.1/src/escape.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/lexer.rs` & `antsi-0.2.1/src/lexer.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/lib.rs` & `antsi-0.2.1/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 use pyo3::exceptions::PyTypeError;
 use pyo3::{create_exception, exceptions::PyException, prelude::*};
-use textwrap::Options;
+use textwrap::Options as WrapOptions;
 
 #[cfg(test)]
 #[macro_use]
 mod macros;
 mod ast;
 mod color;
 mod error;
 mod escape;
 mod lexer;
 mod parser;
 
-use color::colorize;
+use color::{colorize, Options};
 use error::ErrorReport;
 use escape::escape;
 
 create_exception!(
     antsi,
     ColorizeError,
     PyException,
@@ -100,25 +100,30 @@
 /// # Notes
 ///
 /// - If tags are repeated in a style specifier, the value of the last tag takes precedence
 /// - When nesting styled markup, styles of the parent will be applied unless overridden
 /// - There is currently no way to remove text decorations from the children of nested markup
 #[pyfunction]
 #[pyo3(name = "colorize")]
-#[pyo3(signature = (source, file="inline", wrap=None))]
-fn py_colorize(source: &str, file: &str, wrap: Option<usize>) -> PyResult<String> {
+#[pyo3(signature = (source, file="inline", wrap=None, supports_color=true))]
+fn py_colorize(
+    source: &str,
+    file: &str,
+    wrap: Option<usize>,
+    supports_color: bool,
+) -> PyResult<String> {
     if let Some(0) = wrap {
         return Err(PyTypeError::new_err("wrap width must be greater than 0"));
     }
 
-    let styled = colorize(source)
+    let styled = colorize(source, Options { supports_color })
         .map_err(|errors| ColorizeError::from_report(errors.into(), source, file))?;
 
     Ok(match wrap {
-        Some(width) => textwrap::fill(&styled, Options::new(width)),
+        Some(width) => textwrap::fill(&styled, WrapOptions::new(width)),
         None => styled,
     })
 }
 
 /// Escape all styled markup in a piece of text
 #[pyfunction]
 #[pyo3(name = "escape")]
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_13ce0_3q_/tmpqandmifc_TarContainer/0/23.rs", line 138, column 0: CDATA terminal not found*

```diff
@@ -1,16 +1,16 @@
 use pyo3::exceptions::PyTypeError; use pyo3::{create_exception, exceptions::
-PyException, prelude::*}; use textwrap::Options; #[cfg(test)] #[macro_use] mod
-macros; mod ast; mod color; mod error; mod escape; mod lexer; mod parser; use
-color::colorize; use error::ErrorReport; use escape::escape; create_exception!
-( antsi, ColorizeError, PyException, "A report of all the issues found when
-applying styling to a piece of text" ); impl ColorizeError { /// Create a new
-error from a report fn from_report(report: ErrorReport, source: &str, file:
-&str) -> PyErr { match report.emit(file, source, false) { Ok(formatted) =>
-Self::new_err(formatted), Err(e) => PyErr::from(e), } } } /// Convert styled
-markup to ANSI escape codes. /// /// Converts styled markup within the source
-text to ANSI escape codes allowing text to be formatted /// on the command
-line. If a string has no styled markup, it will be passed through unchanged.
-Any /// invalid/unparseable markup will cause an exception. /// /// Text
-wrapping is also supported when the `wrap` parameter is passed with the desired
-width. The /// wrap width must be greater than zero. /// /// Styled markup is
-defined as follows: /// ```text /// [
+PyException, prelude::*}; use textwrap::Options as WrapOptions; #[cfg(test)] #
+[macro_use] mod macros; mod ast; mod color; mod error; mod escape; mod lexer;
+mod parser; use color::{colorize, Options}; use error::ErrorReport; use
+escape::escape; create_exception!( antsi, ColorizeError, PyException, "A report
+of all the issues found when applying styling to a piece of text" ); impl
+ColorizeError { /// Create a new error from a report fn from_report(report:
+ErrorReport, source: &str, file: &str) -> PyErr { match report.emit(file,
+source, false) { Ok(formatted) => Self::new_err(formatted), Err(e) => PyErr::
+from(e), } } } /// Convert styled markup to ANSI escape codes. /// /// Converts
+styled markup within the source text to ANSI escape codes allowing text to be
+formatted /// on the command line. If a string has no styled markup, it will be
+passed through unchanged. Any /// invalid/unparseable markup will cause an
+exception. /// /// Text wrapping is also supported when the `wrap` parameter is
+passed with the desired width. The /// wrap width must be greater than zero. //
+/ /// Styled markup is defined as follows: /// ```text /// [
```

### Comparing `antsi-0.2.0/src/macros.rs` & `antsi-0.2.1/src/macros.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/content.rs` & `antsi-0.2.1/src/parser/content.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/markup.rs` & `antsi-0.2.1/src/parser/markup.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap` & `antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap` & `antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap` & `antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap` & `antsi-0.2.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap` & `antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap` & `antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap` & `antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap` & `antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap` & `antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap` & `antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap` & `antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap` & `antsi-0.2.1/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/style.rs` & `antsi-0.2.1/src/parser/style.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser/text.rs` & `antsi-0.2.1/src/parser/text.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/parser.rs` & `antsi-0.2.1/src/parser.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/snapshots/antsi__lexer__tests__many_tokens.snap` & `antsi-0.2.1/src/snapshots/antsi__lexer__tests__many_tokens.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/snapshots/antsi__lexer__tests__mixed_whitespace_and_text.snap` & `antsi-0.2.1/src/snapshots/antsi__lexer__tests__mixed_whitespace_and_text.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/snapshots/antsi__parser__tests__kitchen_sink.snap` & `antsi-0.2.1/src/snapshots/antsi__parser__tests__kitchen_sink.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/snapshots/antsi__parser__tests__nested_token.snap` & `antsi-0.2.1/src/snapshots/antsi__parser__tests__nested_token.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap` & `antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap` & `antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_token@errors.snap` & `antsi-0.2.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_token@errors.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/Cargo.lock` & `antsi-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "antsi"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "codespan-reporting",
  "indexmap",
  "insta",
  "logos",
  "pyo3",
  "termcolor",
```

### Comparing `antsi-0.2.0/pyproject.toml` & `antsi-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `antsi-0.2.0/PKG-INFO` & `antsi-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: antsi
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md
 Summary: A quick and user-friendly way to style your text using ANSI codes
 Author-email: Alex Krantz <alex@krantz.dev>
 License: MIT
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_13ce0_3q_/tmpqandmifc_TarContainer/0/93", line 200, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: antsi Version: 0.2.0 Classifier: Programming
+Metadata-Version: 2.3 Name: antsi Version: 0.2.1 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md Summary: A quick and user-friendly way to style your
 text using ANSI codes Author-email: Alex Krantz
 krantz.dev> License: MIT Requires-Python: >=3.10 Description-Content-Type:
 text/markdown; charset=UTF-8; variant=GFM Project-URL: homepage, https://
 github.com/akrantz01/antsi Project-URL: issues, https://github.com/akrantz01/
```

