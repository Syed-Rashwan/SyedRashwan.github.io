# SyedRashwan.github.io

## Might make a personalized website. (*^_^*) 
#### Soon? ○( ＾皿＾)っ Hehehe…

  ```
import random

class TimePrediction:
    def __init__(self, possible_times=None):
        if possible_times is None:
            possible_times = ["not tomorrow", "meh", "never"]
        self.possible_times = possible_times

    def _select_time(self):
        try:
            return random.choice(self.possible_times)
        except IndexError:
            raise ValueError("No possible times to choose from.")

    def predict_time(self):
        try:
            when = self._select_time()
            print(f"Soon is {when}.")
        except ValueError as e:
            print(f"Error: {e}")

time_predictor = TimePrediction()
time_predictor.predict_time()
 
  ```
