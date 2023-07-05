# Comparing `tmp/pgn2data-0.0.8.tar.gz` & `tmp/pgn2data-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgn2data-0.0.8.tar", last modified: Fri Oct 28 21:47:42 2022, max compression
+gzip compressed data, was "pgn2data-0.0.9.tar", last modified: Wed Jul  5 12:18:11 2023, max compression
```

## Comparing `pgn2data-0.0.8.tar` & `pgn2data-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-10-28 21:47:42.020606 pgn2data-0.0.8/
--rw-rw-rw-   0        0        0    35823 2022-10-28 20:12:43.000000 pgn2data-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     9150 2022-10-28 21:47:42.020606 pgn2data-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     8102 2022-10-28 21:29:35.000000 pgn2data-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-10-28 21:47:41.989434 pgn2data-0.0.8/common/
--rw-rw-rw-   0        0        0     2085 2022-10-28 20:12:43.000000 pgn2data-0.0.8/common/common.py
--rw-rw-rw-   0        0        0     1079 2022-10-28 20:12:43.000000 pgn2data-0.0.8/common/log_time.py
-drwxrwxrwx   0        0        0        0 2022-10-28 21:47:42.004985 pgn2data-0.0.8/converter/
--rw-rw-rw-   0        0        0        0 2022-10-28 20:12:43.000000 pgn2data-0.0.8/converter/__init__.py
--rw-rw-rw-   0        0        0     3804 2022-10-28 20:12:43.000000 pgn2data-0.0.8/converter/board_ref.py
--rw-rw-rw-   0        0        0     4843 2022-10-28 20:12:43.000000 pgn2data-0.0.8/converter/fen.py
--rw-rw-rw-   0        0        0     3859 2022-10-28 20:12:43.000000 pgn2data-0.0.8/converter/headers.py
--rw-rw-rw-   0        0        0     4753 2022-10-28 20:12:43.000000 pgn2data-0.0.8/converter/pgn_data.py
--rw-rw-rw-   0        0        0    13633 2022-10-28 21:21:58.000000 pgn2data-0.0.8/converter/process.py
--rw-rw-rw-   0        0        0     2379 2022-10-28 20:12:43.000000 pgn2data-0.0.8/converter/result.py
-drwxrwxrwx   0        0        0        0 2022-10-28 21:47:42.020606 pgn2data-0.0.8/pgn2data.egg-info/
--rw-rw-rw-   0        0        0     9150 2022-10-28 21:47:41.000000 pgn2data-0.0.8/pgn2data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2022-10-28 21:47:41.000000 pgn2data-0.0.8/pgn2data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-28 21:47:41.000000 pgn2data-0.0.8/pgn2data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-10-28 21:47:41.000000 pgn2data-0.0.8/pgn2data.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2022-10-28 21:47:41.000000 pgn2data-0.0.8/pgn2data.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-28 21:47:42.020606 pgn2data-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1333 2022-10-28 21:23:41.000000 pgn2data-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-28 21:47:42.020606 pgn2data-0.0.8/testing/
--rw-rw-rw-   0        0        0    11522 2022-10-28 21:18:16.000000 pgn2data-0.0.8/testing/test.py
+drwxrwxrwx   0        0        0        0 2023-07-05 12:18:11.894221 pgn2data-0.0.9/
+-rw-rw-rw-   0        0        0    35823 2023-07-04 15:26:51.000000 pgn2data-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     9761 2023-07-05 12:18:11.894221 pgn2data-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8702 2023-07-04 23:59:01.000000 pgn2data-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 12:18:11.847360 pgn2data-0.0.9/common/
+-rw-rw-rw-   0        0        0     2085 2023-07-04 15:26:51.000000 pgn2data-0.0.9/common/common.py
+-rw-rw-rw-   0        0        0     1079 2023-07-04 15:26:51.000000 pgn2data-0.0.9/common/log_time.py
+drwxrwxrwx   0        0        0        0 2023-07-05 12:18:11.878601 pgn2data-0.0.9/converter/
+-rw-rw-rw-   0        0        0        0 2023-07-04 15:26:51.000000 pgn2data-0.0.9/converter/__init__.py
+-rw-rw-rw-   0        0        0     3804 2023-07-04 15:26:51.000000 pgn2data-0.0.9/converter/board_ref.py
+-rw-rw-rw-   0        0        0     4843 2023-07-04 15:26:51.000000 pgn2data-0.0.9/converter/fen.py
+-rw-rw-rw-   0        0        0     3859 2023-07-04 15:26:51.000000 pgn2data-0.0.9/converter/headers.py
+-rw-rw-rw-   0        0        0     6874 2023-07-05 11:52:33.000000 pgn2data-0.0.9/converter/pgn_data.py
+-rw-rw-rw-   0        0        0    14952 2023-07-04 23:14:47.000000 pgn2data-0.0.9/converter/process.py
+-rw-rw-rw-   0        0        0     2493 2023-07-04 23:40:23.000000 pgn2data-0.0.9/converter/result.py
+drwxrwxrwx   0        0        0        0 2023-07-05 12:18:11.894221 pgn2data-0.0.9/pgn2data.egg-info/
+-rw-rw-rw-   0        0        0     9761 2023-07-05 12:18:11.000000 pgn2data-0.0.9/pgn2data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-07-05 12:18:11.000000 pgn2data-0.0.9/pgn2data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 12:18:11.000000 pgn2data-0.0.9/pgn2data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-05 12:18:11.000000 pgn2data-0.0.9/pgn2data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-05 12:18:11.000000 pgn2data-0.0.9/pgn2data.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 12:18:11.894221 pgn2data-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1349 2023-07-04 23:15:56.000000 pgn2data-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 12:18:11.894221 pgn2data-0.0.9/testing/
+-rw-rw-rw-   0        0        0    17581 2023-07-05 11:59:10.000000 pgn2data-0.0.9/testing/test.py
```

### Comparing `pgn2data-0.0.8/LICENSE` & `pgn2data-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pgn2data-0.0.8/PKG-INFO` & `pgn2data-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pgn2data
-Version: 0.0.8
+Version: 0.0.9
 Summary: Converts a chess pgn file into a csv dataset containing game information and move information
 Home-page: https://github.com/zq99/pgn2data
 Author: zq99
 Author-email: zq99@hotmail.com
 License: GPL-3.0+
-Keywords: CHESS,PGN,NOTATION,DATA,FORSYTH–EDWARDS NOTATION,CSV,DATASET,DATABASE,NORMALIZATION,TABULATION,STRUCTURED DATA,SQL,TABLE,EXCEL
+Keywords: CHESS,PGN,NOTATION,DATA,FORSYTH–EDWARDS NOTATION,CSV,DATASET,DATABASE,NORMALIZATION,TABULATION,STRUCTURED DATA,SQL,TABLE,EXCEL,PYTHON-CHESS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -18,14 +18,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
 
 # pgn2data
 
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+![GitHub stars](https://img.shields.io/github/stars/zq99/pgn2data?style=social)
+![GitHub forks](https://img.shields.io/github/forks/zq99/pgn2data?style=social)
+
+
 This library converts chess pgn files into CSV tabulated data sets.
 
 A pgn file can contain one or multiple chess games. The library parses the pgn file and creates two csv files:
 
 - Games file: contains high level information (e.g. date, site, event, score, players etc...)
 
 - Moves file: contains the moves for each game  (e.g. notation, squares, fen position, is in check etc...)
@@ -85,14 +90,21 @@
         moves_df = result.get_moves_df()
         print(moves_df.head())
         
         # read both files joined together
         combined_df = result.get_combined_df()
         print(combined_df.head())
 
+To output the game information only, you can do the following:
+    
+    from converter.pgn_data import PGNData
+    
+    pgn_data = PGNData("tal_bronstein_1982.pgn")
+    pgn_data.export(moves_required=False)
+
 
 ## Examples
 
 The folder 'samples' in this repository, has some examples of the output from the library.
 
 You can also go [here](https://www.kaggle.com/datasets/zq1200/magnus-carlsen-lichess-games-dataset) to see a Kaggle project that converted all of Magnus Carlsen's online Bullet games
 into CSV format. 
@@ -151,35 +163,38 @@
 | to_square                      | Piece location after                                                    |
 | piece                          | Initial of piece name                                                   |
 | color                          | Piece color                                                             |
 | fen                            | Fen position                                                            |
 | is_check                       | Is check on board                                                       |
 | is_check_mate                  | Is checkmate on board                                                   |
 | is_fifty_moves                 | Is 50 move complete                                                     |
-| is_fivefold_repetition         | Is 5 fold reptition on board                                            |
+| is_fivefold_repetition         | Is 5 fold repetition on board                                           |
 | is_game_over                   | Is game over                                                            |
 | is_insufficient_material       | Is game over from lack of mating material                               |
 | white_count                    | Count of white pieces                                                   |
 | black_count                    | Count of black pieces                                                   |
-| white_{piece}_count            | Count of white specifed piece                                           |
-| black_{piece}_count            | Count of black specifed piece                                           |
+| white_{piece}_count            | Count of white specified piece                                          |
+| black_{piece}_count            | Count of black specified piece                                          |
 | captured_score_for_white       | Total of black pieces captured                                          |
 | captured_score_for_black       | Total of white pieces captured                                          |
 | fen_row{number}_{colour)_count | Number of pieces for the specified colour on this row of the board      |
 | fen_row{number}_{colour}_value | Total value of pieces for the specified colour on this row of the board |
-| move_sequence                  | Sequence of moves upto current position                                 |
+| move_sequence                  | Sequence of moves up to current position                                |
 
 
 ## Contributions
 
 Contributions are welcome, all modifications should come with appropriate tests demonstrating
-an issue has been resolved, or new functionality is working as intended.
+an issue has been resolved, or new functionality is working as intended. Pull Requests without tests
+will not be merged.
 
-All tests can be run by doing the following:
+The library can be tested by doing the following:
 
     from testing.tests import run_all_tests
     run_all_tests()
 
+New tests should be added to the above method.
+
 
 ## Acknowledgements
 
 This project makes use of the [python-chess](https://github.com/niklasf/python-chess) library.
```

### Comparing `pgn2data-0.0.8/README.md` & `pgn2data-0.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # pgn2data
 
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+![GitHub stars](https://img.shields.io/github/stars/zq99/pgn2data?style=social)
+![GitHub forks](https://img.shields.io/github/forks/zq99/pgn2data?style=social)
+
+
 This library converts chess pgn files into CSV tabulated data sets.
 
 A pgn file can contain one or multiple chess games. The library parses the pgn file and creates two csv files:
 
 - Games file: contains high level information (e.g. date, site, event, score, players etc...)
 
 - Moves file: contains the moves for each game  (e.g. notation, squares, fen position, is in check etc...)
@@ -63,14 +68,21 @@
         moves_df = result.get_moves_df()
         print(moves_df.head())
         
         # read both files joined together
         combined_df = result.get_combined_df()
         print(combined_df.head())
 
+To output the game information only, you can do the following:
+    
+    from converter.pgn_data import PGNData
+    
+    pgn_data = PGNData("tal_bronstein_1982.pgn")
+    pgn_data.export(moves_required=False)
+
 
 ## Examples
 
 The folder 'samples' in this repository, has some examples of the output from the library.
 
 You can also go [here](https://www.kaggle.com/datasets/zq1200/magnus-carlsen-lichess-games-dataset) to see a Kaggle project that converted all of Magnus Carlsen's online Bullet games
 into CSV format. 
@@ -129,35 +141,38 @@
 | to_square                      | Piece location after                                                    |
 | piece                          | Initial of piece name                                                   |
 | color                          | Piece color                                                             |
 | fen                            | Fen position                                                            |
 | is_check                       | Is check on board                                                       |
 | is_check_mate                  | Is checkmate on board                                                   |
 | is_fifty_moves                 | Is 50 move complete                                                     |
-| is_fivefold_repetition         | Is 5 fold reptition on board                                            |
+| is_fivefold_repetition         | Is 5 fold repetition on board                                           |
 | is_game_over                   | Is game over                                                            |
 | is_insufficient_material       | Is game over from lack of mating material                               |
 | white_count                    | Count of white pieces                                                   |
 | black_count                    | Count of black pieces                                                   |
-| white_{piece}_count            | Count of white specifed piece                                           |
-| black_{piece}_count            | Count of black specifed piece                                           |
+| white_{piece}_count            | Count of white specified piece                                          |
+| black_{piece}_count            | Count of black specified piece                                          |
 | captured_score_for_white       | Total of black pieces captured                                          |
 | captured_score_for_black       | Total of white pieces captured                                          |
 | fen_row{number}_{colour)_count | Number of pieces for the specified colour on this row of the board      |
 | fen_row{number}_{colour}_value | Total value of pieces for the specified colour on this row of the board |
-| move_sequence                  | Sequence of moves upto current position                                 |
+| move_sequence                  | Sequence of moves up to current position                                |
 
 
 ## Contributions
 
 Contributions are welcome, all modifications should come with appropriate tests demonstrating
-an issue has been resolved, or new functionality is working as intended.
+an issue has been resolved, or new functionality is working as intended. Pull Requests without tests
+will not be merged.
 
-All tests can be run by doing the following:
+The library can be tested by doing the following:
 
     from testing.tests import run_all_tests
     run_all_tests()
 
+New tests should be added to the above method.
+
 
 ## Acknowledgements
 
-This project makes use of the [python-chess](https://github.com/niklasf/python-chess) library.
+This project makes use of the [python-chess](https://github.com/niklasf/python-chess) library.
```

### Comparing `pgn2data-0.0.8/common/common.py` & `pgn2data-0.0.9/common/common.py`

 * *Files identical despite different names*

### Comparing `pgn2data-0.0.8/common/log_time.py` & `pgn2data-0.0.9/common/log_time.py`

 * *Files identical despite different names*

### Comparing `pgn2data-0.0.8/converter/board_ref.py` & `pgn2data-0.0.9/converter/board_ref.py`

 * *Files identical despite different names*

### Comparing `pgn2data-0.0.8/converter/fen.py` & `pgn2data-0.0.9/converter/fen.py`

 * *Files identical despite different names*

### Comparing `pgn2data-0.0.8/converter/headers.py` & `pgn2data-0.0.9/converter/headers.py`

 * *Files identical despite different names*

### Comparing `pgn2data-0.0.8/converter/process.py` & `pgn2data-0.0.9/converter/process.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 log = logging.getLogger("pgn2data - process")
 logging.basicConfig(level=logging.INFO)
 
 
 class PlayerMove:
     """
-    data class to hold details of each move
+    PlayerMove = Data class to hold details of each move.
     move = Move object from python chess library
     notation = is algebraic notation of the move
     """
 
     def __init__(self, move, notation):
         self.move = move
         self.notation = notation
@@ -46,35 +46,70 @@
 
 
 class Process:
     """
     Handles the pgn to data conversion
     """
 
-    def __init__(self, pgn_file, file_games, file_moves, engine_path, engine_depth):
+    def __init__(self, pgn_file, file_games, file_moves, engine_path, engine_depth, moves_required, queue_size=0):
         self.pgn_file = pgn_file
         self.file_games = file_games
         self.file_moves = file_moves
         self.engine_path = engine_path
         self.engine_depth = engine_depth
+        self.max_queue_size = queue_size
+        self.moves_required = moves_required
 
     def parse_file(self, add_headers_flag=True):
         """
-        processes on pgn file and then exports game information
+        This is the main method of the class for invoking the file processing
+        """
+
+        if self.moves_required:
+            self.__parse_file_games_and_moves(add_headers_flag)
+        else:
+            self.__parse_file_games(add_headers_flag)
+
+    def __parse_file_games(self, add_headers_flag=True):
+        """
+        processes the pgn file and then exports game information
+        into the game csv file, moves are ignored
+        """
+
+        log.info("Processing games only in file:{}".format(self.pgn_file))
+        pgn = open(self.pgn_file, encoding="UTF-8")
+
+        game_writer = csv.writer(self.file_games, delimiter=',')
+        if add_headers_flag:
+            game_writer.writerow(file_headers_game)
+
+        order = 1
+        while True:
+            game_id = str(uuid.uuid4())
+            game = chess.pgn.read_game(pgn)
+            if game is None:
+                break  # end of file
+
+            game_writer.writerow(self.__get_game_row_data(game, game_id, order, self.pgn_file))
+            order += 1
+
+    def __parse_file_games_and_moves(self, add_headers_flag=True):
+        """
+        processes the pgn file and then exports game information
         into the game csv file, and the moves into the moves csv file
         """
 
-        log.info("Processing file:{}".format(self.pgn_file))
+        log.info("Processing games and moves in file:{}".format(self.pgn_file))
         pgn = open(self.pgn_file, encoding="UTF-8")
 
         engine = None
         if self.engine_path is not None:
             engine = chess.engine.SimpleEngine.popen_uci(self.engine_path)
 
-        q = queue.Queue(maxsize=0)
+        q = queue.Queue(maxsize=self.max_queue_size)
         worker = Thread(target=self.__process_move_queue, args=(q,))
         worker.setDaemon(True)
         worker.start()
 
         move_writer = csv.writer(self.file_moves, delimiter=',')
         if add_headers_flag:
             headers = file_headers_moves
```

### Comparing `pgn2data-0.0.8/converter/result.py` & `pgn2data-0.0.9/converter/result.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,33 +23,38 @@
 
     def print_summary(self):
         """
         return a summary to console
         """
         print("is complete: {}".format(str(self.is_complete)))
         print("games file: {} | size: {}".format(self.games_file.name, self.games_file.size))
-        print("moves file: {} | size: {}".format(self.moves_file.name, self.moves_file.size))
+        if self.moves_file is not None:
+            print("moves file: {} | size: {}".format(self.moves_file.name, self.moves_file.size))
 
     def get_games_df(self):
         return self.__get_as_dataframe(self.games_file.name)
 
     def get_moves_df(self):
-        return self.__get_as_dataframe(self.moves_file.name)
+        if self.moves_file is None:
+            return None
+        else:
+            return self.__get_as_dataframe(self.moves_file.name)
 
     def get_combined_df(self):
         games_df = self.get_games_df()
         moves_df = self.get_moves_df()
-        if (games_df is not None) and (moves_df is not None):
-            if (not games_df.empty) and (not moves_df.empty):
+
+        if (games_df is not None) and (not games_df.empty):
+            if (moves_df is not None) and (not moves_df.empty):
                 combined_df = pd.merge(games_df, moves_df, on='game_id')
                 return combined_df
             else:
-                log.error("one or both files is empty")
+                return games_df
         else:
-            log.error("one or both files not found")
+            log.error("games information is missing or empty")
         return None
 
     def create_combined_file(self, filename):
         combined_df = self.get_combined_df()
         if combined_df is not None:
             combined_df.to_csv(filename, index=False)
             return os.path.exists(filename)
```

### Comparing `pgn2data-0.0.8/pgn2data.egg-info/PKG-INFO` & `pgn2data-0.0.9/pgn2data.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pgn2data
-Version: 0.0.8
+Version: 0.0.9
 Summary: Converts a chess pgn file into a csv dataset containing game information and move information
 Home-page: https://github.com/zq99/pgn2data
 Author: zq99
 Author-email: zq99@hotmail.com
 License: GPL-3.0+
-Keywords: CHESS,PGN,NOTATION,DATA,FORSYTH–EDWARDS NOTATION,CSV,DATASET,DATABASE,NORMALIZATION,TABULATION,STRUCTURED DATA,SQL,TABLE,EXCEL
+Keywords: CHESS,PGN,NOTATION,DATA,FORSYTH–EDWARDS NOTATION,CSV,DATASET,DATABASE,NORMALIZATION,TABULATION,STRUCTURED DATA,SQL,TABLE,EXCEL,PYTHON-CHESS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -18,14 +18,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
 
 # pgn2data
 
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+![GitHub stars](https://img.shields.io/github/stars/zq99/pgn2data?style=social)
+![GitHub forks](https://img.shields.io/github/forks/zq99/pgn2data?style=social)
+
+
 This library converts chess pgn files into CSV tabulated data sets.
 
 A pgn file can contain one or multiple chess games. The library parses the pgn file and creates two csv files:
 
 - Games file: contains high level information (e.g. date, site, event, score, players etc...)
 
 - Moves file: contains the moves for each game  (e.g. notation, squares, fen position, is in check etc...)
@@ -85,14 +90,21 @@
         moves_df = result.get_moves_df()
         print(moves_df.head())
         
         # read both files joined together
         combined_df = result.get_combined_df()
         print(combined_df.head())
 
+To output the game information only, you can do the following:
+    
+    from converter.pgn_data import PGNData
+    
+    pgn_data = PGNData("tal_bronstein_1982.pgn")
+    pgn_data.export(moves_required=False)
+
 
 ## Examples
 
 The folder 'samples' in this repository, has some examples of the output from the library.
 
 You can also go [here](https://www.kaggle.com/datasets/zq1200/magnus-carlsen-lichess-games-dataset) to see a Kaggle project that converted all of Magnus Carlsen's online Bullet games
 into CSV format. 
@@ -151,35 +163,38 @@
 | to_square                      | Piece location after                                                    |
 | piece                          | Initial of piece name                                                   |
 | color                          | Piece color                                                             |
 | fen                            | Fen position                                                            |
 | is_check                       | Is check on board                                                       |
 | is_check_mate                  | Is checkmate on board                                                   |
 | is_fifty_moves                 | Is 50 move complete                                                     |
-| is_fivefold_repetition         | Is 5 fold reptition on board                                            |
+| is_fivefold_repetition         | Is 5 fold repetition on board                                           |
 | is_game_over                   | Is game over                                                            |
 | is_insufficient_material       | Is game over from lack of mating material                               |
 | white_count                    | Count of white pieces                                                   |
 | black_count                    | Count of black pieces                                                   |
-| white_{piece}_count            | Count of white specifed piece                                           |
-| black_{piece}_count            | Count of black specifed piece                                           |
+| white_{piece}_count            | Count of white specified piece                                          |
+| black_{piece}_count            | Count of black specified piece                                          |
 | captured_score_for_white       | Total of black pieces captured                                          |
 | captured_score_for_black       | Total of white pieces captured                                          |
 | fen_row{number}_{colour)_count | Number of pieces for the specified colour on this row of the board      |
 | fen_row{number}_{colour}_value | Total value of pieces for the specified colour on this row of the board |
-| move_sequence                  | Sequence of moves upto current position                                 |
+| move_sequence                  | Sequence of moves up to current position                                |
 
 
 ## Contributions
 
 Contributions are welcome, all modifications should come with appropriate tests demonstrating
-an issue has been resolved, or new functionality is working as intended.
+an issue has been resolved, or new functionality is working as intended. Pull Requests without tests
+will not be merged.
 
-All tests can be run by doing the following:
+The library can be tested by doing the following:
 
     from testing.tests import run_all_tests
     run_all_tests()
 
+New tests should be added to the above method.
+
 
 ## Acknowledgements
 
 This project makes use of the [python-chess](https://github.com/niklasf/python-chess) library.
```

### Comparing `pgn2data-0.0.8/setup.py` & `pgn2data-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,24 +10,24 @@
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
 ]
 
 setup(
     name='pgn2data',
-    version='0.0.8',
+    version='0.0.9',
     packages=['converter', 'common', 'testing'],
     url='https://github.com/zq99/pgn2data',
     python_requires=">=3.7",
     classifiers=classifiers,
     license='GPL-3.0+',
     author='zq99',
     author_email='zq99@hotmail.com',
     keywords=['CHESS', 'PGN', 'NOTATION', 'DATA', 'FORSYTH–EDWARDS NOTATION', 'CSV', 'DATASET', 'DATABASE',
-              'NORMALIZATION', 'TABULATION', 'STRUCTURED DATA', 'SQL', 'TABLE', 'EXCEL'],
+              'NORMALIZATION', 'TABULATION', 'STRUCTURED DATA', 'SQL', 'TABLE', 'EXCEL', 'PYTHON-CHESS'],
     install_requires=[
         'chess',
         'pandas'
     ],
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown; charset=UTF-8; variant=GFM',
     description='Converts a chess pgn file into a csv dataset containing game information and move information',
```

