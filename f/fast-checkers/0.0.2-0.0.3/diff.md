# Comparing `tmp/fast-checkers-0.0.2.tar.gz` & `tmp/fast-checkers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-checkers-0.0.2.tar", last modified: Tue Jul  4 22:18:46 2023, max compression
+gzip compressed data, was "fast-checkers-0.0.3.tar", last modified: Wed Jul  5 11:56:40 2023, max compression
```

## Comparing `fast-checkers-0.0.2.tar` & `fast-checkers-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:46.825040 fast-checkers-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-04 22:18:46.825040 fast-checkers-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:46.825040 fast-checkers-0.0.2/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/checkers/american_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/checkers/base_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/checkers/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/checkers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/checkers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:46.825040 fast-checkers-0.0.2/fast_checkers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-04 22:18:46.000000 fast-checkers-0.0.2/fast_checkers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-04 22:18:46.000000 fast-checkers-0.0.2/fast_checkers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:18:46.000000 fast-checkers-0.0.2/fast_checkers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 22:18:46.000000 fast-checkers-0.0.2/fast_checkers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 22:18:46.825040 fast-checkers-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:46.825040 fast-checkers-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-05 11:56:40.357052 fast-checkers-0.0.3/
+-rw-rw-rw-   0        0        0     2711 2023-07-05 11:56:40.355051 fast-checkers-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2169 2023-07-05 07:52:18.000000 fast-checkers-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 11:56:40.316189 fast-checkers-0.0.3/checkers/
+-rw-rw-rw-   0        0        0     1516 2023-07-05 07:52:01.000000 fast-checkers-0.0.3/checkers/__init__.py
+-rw-rw-rw-   0        0        0     3552 2023-07-05 07:48:08.000000 fast-checkers-0.0.3/checkers/american_board.py
+-rw-rw-rw-   0        0        0     4276 2023-07-05 07:48:34.000000 fast-checkers-0.0.3/checkers/base_board.py
+-rw-rw-rw-   0        0        0     1161 2023-07-05 07:25:47.000000 fast-checkers-0.0.3/checkers/main.py
+-rw-rw-rw-   0        0        0     3357 2023-07-05 07:36:27.000000 fast-checkers-0.0.3/checkers/models.py
+-rw-rw-rw-   0        0        0       65 2023-07-04 07:53:40.000000 fast-checkers-0.0.3/checkers/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-05 11:56:40.342033 fast-checkers-0.0.3/fast_checkers.egg-info/
+-rw-rw-rw-   0        0        0     2711 2023-07-05 11:56:36.000000 fast-checkers-0.0.3/fast_checkers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-05 11:56:39.000000 fast-checkers-0.0.3/fast_checkers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 11:56:36.000000 fast-checkers-0.0.3/fast_checkers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-05 11:56:36.000000 fast-checkers-0.0.3/fast_checkers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 11:56:40.358055 fast-checkers-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      829 2023-07-05 11:52:26.000000 fast-checkers-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 11:56:40.350051 fast-checkers-0.0.3/test/
+-rw-rw-rw-   0        0        0     2376 2023-07-05 07:24:56.000000 fast-checkers-0.0.3/test/test_board.py
```

### Comparing `fast-checkers-0.0.2/checkers/american_board.py` & `fast-checkers-0.0.3/checkers/american_board.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-from __future__ import annotations
-from typing import Generator
-from checkers.base_board import BaseBoard
-from checkers.models import STARTING_POSITION, Move, Color, Entity
-from checkers.utils import logger
-import checkers
-import numpy as np
-
-"""
- board 8x8
- Short moves only 
- Cannot capture backwards
- Capture - choose any
-"""
-
-
-class AmericanBoard(BaseBoard):
-    STARTING_POSITION = np.array([1] * 12 + [0] * 8 + [-1] * 12, dtype=np.int8)
-    size = int(np.sqrt(len(STARTING_POSITION) * 2))
-    row_idx = {val: val // 4 for val in range(len(STARTING_POSITION))}
-    col_idx = {val: val % 8 for val in range(len(STARTING_POSITION))}
-
-    @property
-    def legal_moves(self) -> Generator[Move, None, None]:
-        if self.turn == Color.BLACK:
-            squares_list = np.transpose(np.nonzero(self._pos > 0))
-        else:
-            squares_list = np.transpose(np.nonzero(self._pos < 0))
-
-        for square in squares_list.flatten():
-            moves = self._legal_moves_from(square)
-            for move in moves:
-                yield move
-
-    def _legal_moves_from(self, square: int) -> Generator[Move, None, None]:
-        row = self.row_idx[square]
-        moves = []
-        odd = (row % 2 != 0 and self.turn == Color.BLACK) or (
-            row % 2 == 0 and self.turn == Color.WHITE
-        )
-        move_right = square + (4 - odd) * (self.turn.value)
-        capture_right = square + 7 * (self.turn.value)
-        move_left = square + (5 - odd) * (self.turn.value)
-        capture_left = square + 9 * (self.turn.value)
-        if (
-            0 <= move_right < len(self._pos)
-            and row + 1 * (self.turn.value) == self.row_idx[move_right]
-            and self[move_right] == 0
-        ):
-            moves.append(Move([square, move_right]))
-        elif (
-            0 <= capture_right < len(self._pos)
-            and row + 2 * (self.turn.value) == self.row_idx[capture_right]
-            and self[capture_right] == 0
-            and self[move_right] == self.turn.value * -1
-        ):
-            move = Move(
-                [square, capture_right],
-                captured_list=[move_right],
-                captured_entities=[False],
-            )
-            moves.append(move)
-            self.push(move, False)
-            moves += [move + m for m in self._legal_moves_from(capture_right)]
-            self.pop(False)
-        if (
-            0 <= move_left < len(self._pos)
-            and row + 1 * (self.turn.value) == self.row_idx[move_left]
-            and self[move_left] == 0
-        ):
-            moves.append(Move([square, move_left]))
-        elif (
-            0 <= capture_left < len(self._pos)
-            and row + 2 * (self.turn.value) == self.row_idx[capture_left]
-            and self[capture_left] == 0
-            and self[move_left] == self.turn.value * -1
-        ):
-            move = Move(
-                [square, capture_left],
-                captured_list=[move_left],
-                captured_entities=[False],
-            )
-            moves.append(move)
-            self.push(move, False)
-            moves += [move + m for m in self._legal_moves_from(capture_left)]
-            self.pop(False)
-        return moves
-
-
-if __name__ == "__main__":
-    board = AmericanBoard()
-    while True:
-        moves = board.legal_moves
-        move = np.random.choice(list(moves))
-        board.push(move)
-        print(move)
-        print(board)
-        from time import sleep
-
-        sleep(2)
+from __future__ import annotations
+from typing import Generator
+from checkers.base_board import BaseBoard
+from checkers.models import STARTING_POSITION, Move, Color, Entity
+from checkers.utils import logger
+import checkers
+import numpy as np
+
+"""
+ board 8x8
+ Short moves only 
+ Cannot capture backwards
+ Capture - choose any
+"""
+
+
+class AmericanBoard(BaseBoard):
+    STARTING_POSITION = np.array([1] * 12 + [0] * 8 + [-1] * 12, dtype=np.int8)
+    size = int(np.sqrt(len(STARTING_POSITION) * 2))
+    row_idx = {val: val // 4 for val in range(len(STARTING_POSITION))}
+    col_idx = {val: val % 8 for val in range(len(STARTING_POSITION))}
+
+    @property
+    def legal_moves(self) -> Generator[Move, None, None]:
+        if self.turn == Color.BLACK:
+            squares_list = np.transpose(np.nonzero(self._pos > 0))
+        else:
+            squares_list = np.transpose(np.nonzero(self._pos < 0))
+
+        for square in squares_list.flatten():
+            moves = self._legal_moves_from(square)
+            for move in moves:
+                yield move
+
+    def _legal_moves_from(self, square: int) -> Generator[Move, None, None]:
+        row = self.row_idx[square]
+        moves = []
+        odd = (row % 2 != 0 and self.turn == Color.BLACK) or (
+            row % 2 == 0 and self.turn == Color.WHITE
+        )
+        move_right = square + (4 - odd) * (self.turn.value)
+        capture_right = square + 7 * (self.turn.value)
+        move_left = square + (5 - odd) * (self.turn.value)
+        capture_left = square + 9 * (self.turn.value)
+        if (
+            0 <= move_right < len(self._pos)
+            and row + 1 * (self.turn.value) == self.row_idx[move_right]
+            and self[move_right] == 0
+        ):
+            moves.append(Move([square, move_right]))
+        elif (
+            0 <= capture_right < len(self._pos)
+            and row + 2 * (self.turn.value) == self.row_idx[capture_right]
+            and self[capture_right] == 0
+            and self[move_right] == self.turn.value * -1
+        ):
+            move = Move(
+                [square, capture_right],
+                captured_list=[move_right],
+                captured_entities=[False],
+            )
+            moves.append(move)
+            self.push(move, False)
+            moves += [move + m for m in self._legal_moves_from(capture_right)]
+            self.pop(False)
+        if (
+            0 <= move_left < len(self._pos)
+            and row + 1 * (self.turn.value) == self.row_idx[move_left]
+            and self[move_left] == 0
+        ):
+            moves.append(Move([square, move_left]))
+        elif (
+            0 <= capture_left < len(self._pos)
+            and row + 2 * (self.turn.value) == self.row_idx[capture_left]
+            and self[capture_left] == 0
+            and self[move_left] == self.turn.value * -1
+        ):
+            move = Move(
+                [square, capture_left],
+                captured_list=[move_left],
+                captured_entities=[False],
+            )
+            moves.append(move)
+            self.push(move, False)
+            moves += [move + m for m in self._legal_moves_from(capture_left)]
+            self.pop(False)
+        return moves
+
+
+if __name__ == "__main__":
+    board = AmericanBoard()
+    while True:
+        moves = board.legal_moves
+        move = np.random.choice(list(moves))
+        board.push(move)
+        print(move)
+        print(board)
+        from time import sleep
+
+        sleep(2)
```

### Comparing `fast-checkers-0.0.2/checkers/base_board.py` & `fast-checkers-0.0.3/checkers/base_board.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-from __future__ import annotations
-import numpy as np
-from checkers.utils import logger
-from checkers.models import (
-    Entity,
-    ENTITY_REPR,
-    STARTING_POSITION,
-    ENTITY_MAP,
-    Color,
-    Move,
-    SquareT,
-)
-import checkers
-from typing import Generator, Literal
-from abc import ABC, abstractmethod
-import warnings
-
-
-class BaseBoard(ABC):
-    """
-    The class is designed to support checkers boards of any size.
-    The shape attribute, represented as a tuple (rows, columns),
-    enables dynamic configuration of the board's dimensions.
-    """
-
-    SQUARES_MAP: checkers.T10X10 | checkers.T8X8 = checkers.T8X8
-
-    def __init__(self, position: np.ndarray = STARTING_POSITION) -> None:
-        super().__init__()
-        self._pos = position.copy()
-        size = int(np.sqrt(len(self.position) * 2))
-        if size**2 != len(self.position) * 2:
-            msg = f"Invalid board with shape {position.shape} provided.\
-                Please use an array with lenght = (n * n/2). \
-                Where n is an size of the board."
-            logger.error(msg)
-            raise ValueError(msg)
-        self.shape = (size, size)
-        self.turn = Color.WHITE
-        self._moves_stack: list[Move] = []
-        logger.info(f"Board initialized with shape {self.shape}.")
-
-    # @abstractmethod
-    def legal_moves(self) -> Generator[Move, None, None]:
-        pass
-
-    @property
-    def position(self) -> np.ndarray:
-        """Returns board position."""
-        return self._pos
-
-    def push(self, move: Move, is_finished: bool = True) -> None:
-        """Pushes a move to the board."""
-        src, tg = (
-            move.square_list[0],
-            move.square_list[-1],
-        )
-        self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
-        if move.captured_list:
-            self._pos[
-                np.array([self.SQUARES_MAP[sq] for sq in move.captured_list])
-            ] = Entity.EMPTY
-        self._moves_stack.append(move)
-        if is_finished:
-            self.turn = Color.WHITE if self.turn == Color.BLACK else Color.BLACK
-
-    def pop(self, is_finished=True) -> None:
-        """Pops a move from the board."""
-        move = self._moves_stack.pop()
-        src, tg = (
-            move.square_list[0],
-            move.square_list[-1],
-        )
-        self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
-        for sq, is_king in zip(move.captured_list, move.captured_entities):
-            self._pos[sq] = ENTITY_MAP[(self.turn, is_king)]
-        if is_finished:
-            self.turn = Color.WHITE if self.turn == Color.BLACK else Color.BLACK
-        return move
-
-    @property
-    def friendly_form(self) -> np.ndarray:
-        """
-        Really tricky method. It is used to print board in a friendly way.
-        Designed so it can be used with any board size.
-        """
-        new_pos = [0]
-        for idx, sq in enumerate(self.position):
-            new_pos.extend([0] * (idx % (self.shape[0] // 2) != 0))
-            new_pos.extend([0, 0] * (idx % self.shape[0] == 0 and idx != 0))
-            new_pos.append(sq)
-        new_pos.append(0)
-        return np.array(new_pos)
-
-    def __repr__(self) -> str:
-        board = ""
-        position = self.friendly_form
-        for i in range(self.shape[0]):
-            board += f"{'-' * (self.shape[0]*4 + 1) }\n|"
-            for j in range(self.shape[0]):
-                board += f" {ENTITY_REPR[position[i*self.shape[0] + j]]} |"
-            board += "\n"
-        return board
-
-    def __iter__(self) -> Generator[Entity, None, None]:
-        for sq in self.position:
-            yield sq
-
-    def __getitem__(self, key: SquareT) -> Entity:
-        return self.position[key]
-
-
-if __name__ == "__main__":
-    board = BaseBoard(STARTING_POSITION)
-
-    m1 = Move([checkers.C3, checkers.B4])
-    board.push(m1)
-
-    m2 = Move([checkers.B6, checkers.A5])
-    board.push(m2)
-
-    m3 = Move([checkers.G3, checkers.H4])
-    board.push(m3)
-    print(board)
-
-    m4 = Move([checkers.A5, checkers.C3], captured_list=[checkers.B4])
-    board.push(m4)
-    print(board)
-    checkers.SQUARES = range(51)
-    print(checkers.SQUARES)
+from __future__ import annotations
+from checkers.utils import logger
+from checkers.models import (
+    Entity,
+    ENTITY_REPR,
+    STARTING_POSITION,
+    ENTITY_MAP,
+    Color,
+    Move,
+    SquareT,
+)
+import checkers
+from typing import Generator, Literal
+from abc import ABC, abstractmethod
+import warnings
+import numpy as np
+
+
+class BaseBoard(ABC):
+    """
+    The class is designed to support checkers boards of any size.
+    The shape attribute, represented as a tuple (rows, columns),
+    enables dynamic configuration of the board's dimensions.
+    """
+
+    SQUARES_MAP: checkers.T10X10 | checkers.T8X8 = checkers.T8X8
+
+    def __init__(self, position: np.ndarray = STARTING_POSITION) -> None:
+        super().__init__()
+        self._pos = position.copy()
+        size = int(np.sqrt(len(self.position) * 2))
+        if size**2 != len(self.position) * 2:
+            msg = f"Invalid board with shape {position.shape} provided.\
+                Please use an array with lenght = (n * n/2). \
+                Where n is an size of the board."
+            logger.error(msg)
+            raise ValueError(msg)
+        self.shape = (size, size)
+        self.turn = Color.WHITE
+        self._moves_stack: list[Move] = []
+        logger.info(f"Board initialized with shape {self.shape}.")
+
+    # @abstractmethod
+    def legal_moves(self) -> Generator[Move, None, None]:
+        pass
+
+    @property
+    def position(self) -> np.ndarray:
+        """Returns board position."""
+        return self._pos
+
+    def push(self, move: Move, is_finished: bool = True) -> None:
+        """Pushes a move to the board."""
+        src, tg = (
+            move.square_list[0],
+            move.square_list[-1],
+        )
+        self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
+        if move.captured_list:
+            self._pos[
+                np.array([self.SQUARES_MAP[sq] for sq in move.captured_list])
+            ] = Entity.EMPTY
+        self._moves_stack.append(move)
+        if is_finished:
+            self.turn = Color.WHITE if self.turn == Color.BLACK else Color.BLACK
+
+    def pop(self, is_finished=True) -> None:
+        """Pops a move from the board."""
+        move = self._moves_stack.pop()
+        src, tg = (
+            move.square_list[0],
+            move.square_list[-1],
+        )
+        self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
+        for sq, is_king in zip(move.captured_list, move.captured_entities):
+            self._pos[sq] = ENTITY_MAP[(self.turn, is_king)]
+        if is_finished:
+            self.turn = Color.WHITE if self.turn == Color.BLACK else Color.BLACK
+        return move
+
+    @property
+    def friendly_form(self) -> np.ndarray:
+        """
+        Really tricky method. It is used to print board in a friendly way.
+        Designed so it can be used with any board size.
+        """
+        new_pos = [0]
+        for idx, sq in enumerate(self.position):
+            new_pos.extend([0] * (idx % (self.shape[0] // 2) != 0))
+            new_pos.extend([0, 0] * (idx % self.shape[0] == 0 and idx != 0))
+            new_pos.append(sq)
+        new_pos.append(0)
+        return np.array(new_pos)
+
+    def __repr__(self) -> str:
+        board = ""
+        position = self.friendly_form
+        for i in range(self.shape[0]):
+            board += f"{'-' * (self.shape[0]*4 + 1) }\n|"
+            for j in range(self.shape[0]):
+                board += f" {ENTITY_REPR[position[i*self.shape[0] + j]]} |"
+            board += "\n"
+        return board
+
+    def __iter__(self) -> Generator[Entity, None, None]:
+        for sq in self.position:
+            yield sq
+
+    def __getitem__(self, key: SquareT) -> Entity:
+        return self.position[key]
+
+
+if __name__ == "__main__":
+    board = BaseBoard(STARTING_POSITION)
+
+    m1 = Move([checkers.C3, checkers.B4])
+    board.push(m1)
+
+    m2 = Move([checkers.B6, checkers.A5])
+    board.push(m2)
+
+    m3 = Move([checkers.G3, checkers.H4])
+    board.push(m3)
+    print(board)
+
+    m4 = Move([checkers.A5, checkers.C3], captured_list=[checkers.B4])
+    board.push(m4)
+    print(board)
+    checkers.SQUARES = range(51)
+    print(checkers.SQUARES)
```

### Comparing `fast-checkers-0.0.2/checkers/main.py` & `fast-checkers-0.0.3/checkers/main.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import numpy as np
-from fastapi import FastAPI, Request
-import uvicorn
-from fastapi.responses import JSONResponse, HTMLResponse
-from fastapi.templating import Jinja2Templates
-from fastapi.staticfiles import StaticFiles
-from checkers.american_board import AmericanBoard as Board
-
-templates = Jinja2Templates(directory="checkers/templates/")
-
-app = FastAPI()
-board = Board()
-app.mount("/static", StaticFiles(directory="checkers/static"), name="static")
-
-
-@app.get("/")
-def index(request: Request):
-    return templates.TemplateResponse(
-        "index.html",
-        {"request": request, "board": board.friendly_form.reshape(8, 8).tolist()},
-    )
-
-
-@app.get("/random_move")
-def random_move(request: Request):
-    moves = list(board.legal_moves)
-    # get move wiht longest capture chain
-    move = max(moves, key=lambda x: len(x.captured_list))
-    print(move)
-    board.push(move)
-    return {"position": board.friendly_form.reshape(8, 8).tolist()}
-
-
-@app.get("/board")
-def get_board(request: Request):
-    return {"position": board.friendly_form.reshape(8, 8).tolist()}
-
-
-if __name__ == "__main__":
-    uvicorn.run(app)
+import numpy as np
+from fastapi import FastAPI, Request
+import uvicorn
+from fastapi.responses import JSONResponse, HTMLResponse
+from fastapi.templating import Jinja2Templates
+from fastapi.staticfiles import StaticFiles
+from checkers.american_board import AmericanBoard as Board
+
+templates = Jinja2Templates(directory="checkers/templates/")
+
+app = FastAPI()
+board = Board()
+app.mount("/static", StaticFiles(directory="checkers/static"), name="static")
+
+
+@app.get("/")
+def index(request: Request):
+    return templates.TemplateResponse(
+        "index.html",
+        {"request": request, "board": board.friendly_form.reshape(8, 8).tolist()},
+    )
+
+
+@app.get("/random_move")
+def random_move(request: Request):
+    moves = list(board.legal_moves)
+    # get move wiht longest capture chain
+    move = max(moves, key=lambda x: len(x.captured_list))
+    print(move)
+    board.push(move)
+    return {"position": board.friendly_form.reshape(8, 8).tolist()}
+
+
+@app.get("/board")
+def get_board(request: Request):
+    return {"position": board.friendly_form.reshape(8, 8).tolist()}
+
+
+if __name__ == "__main__":
+    uvicorn.run(app)
```

### Comparing `fast-checkers-0.0.2/test/test_board.py` & `fast-checkers-0.0.3/test/test_board.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-from checkers.base_board import (
-    BaseBoard,
-    Color,
-    Move,
-    STARTING_POSITION,
-    Entity,
-)
-import checkers
-import pytest
-import numpy as np
-
-
-class TestBoard:
-    @pytest.fixture(autouse=True)
-    def setup(self):
-        self.board = BaseBoard()
-        yield
-        del self.board
-
-    def test_init(self):
-        assert self.board.turn == Color.WHITE
-        assert np.array_equal(self.board.position, STARTING_POSITION)
-
-    def test_move(self):
-        m = Move([checkers.A3, checkers.B4])
-        self.board.push(m)
-        assert self.board.turn == Color.BLACK
-        assert self.board[checkers.A3] == Entity.EMPTY
-        assert self.board[checkers.B4] == Entity.WHITE_MAN
-        m = Move([checkers.F6, checkers.G5])
-        self.board.push(m)
-        assert self.board.turn == Color.WHITE
-        assert self.board[checkers.F6] == Entity.EMPTY
-        assert self.board[checkers.G5] == Entity.BLACK_MAN
-
-    def test_capture(self):
-        m1 = Move([checkers.C3, checkers.B4])
-        self.board.push(m1)
-
-        m2 = Move([checkers.B6, checkers.A5])
-        self.board.push(m2)
-
-        m3 = Move([checkers.G3, checkers.H4])
-        self.board.push(m3)
-
-        m4 = Move([checkers.A5, checkers.C3], captured_list=[checkers.B4])
-        self.board.push(m4)
-
-        assert self.board[checkers.B4] == Entity.EMPTY
-        assert self.board[checkers.C3] == Entity.BLACK_MAN
-
-        m5 = Move([checkers.B2, checkers.D4], captured_list=[checkers.C3])
-        self.board.push(m5)
-        assert self.board[checkers.B2] == Entity.EMPTY
-        assert self.board[checkers.C3] == Entity.EMPTY
-        assert self.board[checkers.D4] == Entity.WHITE_MAN
-
-    def test_pop(self):
-        m = Move([checkers.A3, checkers.B4])
-        self.board.push(m)
-        assert self.board.turn == Color.BLACK
-        assert self.board[checkers.A3] == Entity.EMPTY
-        assert self.board[checkers.B4] == Entity.WHITE_MAN
-        m = Move([checkers.F6, checkers.G5])
-        self.board.push(m)
-        self.board.pop()
-        assert self.board.turn == Color.BLACK
-        assert self.board[checkers.F6] == Entity.BLACK_MAN
-        assert self.board[checkers.G5] == Entity.EMPTY
-        assert self.board[checkers.A3] == Entity.EMPTY
-        assert self.board[checkers.B4] == Entity.WHITE_MAN
+from checkers.base_board import (
+    BaseBoard,
+    Color,
+    Move,
+    STARTING_POSITION,
+    Entity,
+)
+import checkers
+import pytest
+import numpy as np
+
+
+class TestBoard:
+    @pytest.fixture(autouse=True)
+    def setup(self):
+        self.board = BaseBoard()
+        yield
+        del self.board
+
+    def test_init(self):
+        assert self.board.turn == Color.WHITE
+        assert np.array_equal(self.board.position, STARTING_POSITION)
+
+    def test_move(self):
+        m = Move([checkers.A3, checkers.B4])
+        self.board.push(m)
+        assert self.board.turn == Color.BLACK
+        assert self.board[checkers.A3] == Entity.EMPTY
+        assert self.board[checkers.B4] == Entity.WHITE_MAN
+        m = Move([checkers.F6, checkers.G5])
+        self.board.push(m)
+        assert self.board.turn == Color.WHITE
+        assert self.board[checkers.F6] == Entity.EMPTY
+        assert self.board[checkers.G5] == Entity.BLACK_MAN
+
+    def test_capture(self):
+        m1 = Move([checkers.C3, checkers.B4])
+        self.board.push(m1)
+
+        m2 = Move([checkers.B6, checkers.A5])
+        self.board.push(m2)
+
+        m3 = Move([checkers.G3, checkers.H4])
+        self.board.push(m3)
+
+        m4 = Move([checkers.A5, checkers.C3], captured_list=[checkers.B4])
+        self.board.push(m4)
+
+        assert self.board[checkers.B4] == Entity.EMPTY
+        assert self.board[checkers.C3] == Entity.BLACK_MAN
+
+        m5 = Move([checkers.B2, checkers.D4], captured_list=[checkers.C3])
+        self.board.push(m5)
+        assert self.board[checkers.B2] == Entity.EMPTY
+        assert self.board[checkers.C3] == Entity.EMPTY
+        assert self.board[checkers.D4] == Entity.WHITE_MAN
+
+    def test_pop(self):
+        m = Move([checkers.A3, checkers.B4])
+        self.board.push(m)
+        assert self.board.turn == Color.BLACK
+        assert self.board[checkers.A3] == Entity.EMPTY
+        assert self.board[checkers.B4] == Entity.WHITE_MAN
+        m = Move([checkers.F6, checkers.G5])
+        self.board.push(m)
+        self.board.pop()
+        assert self.board.turn == Color.BLACK
+        assert self.board[checkers.F6] == Entity.BLACK_MAN
+        assert self.board[checkers.G5] == Entity.EMPTY
+        assert self.board[checkers.A3] == Entity.EMPTY
+        assert self.board[checkers.B4] == Entity.WHITE_MAN
```

