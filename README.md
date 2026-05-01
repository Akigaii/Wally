# Wally

A fine-tuned sentence transformer trained on the mechanics of [Wavelength](https://www.boardseyeview.net/post/wavelength) to simulate human semantic reasoning. Wally acts as the "guesser" — given a word pair and a clue, it predicts a value on a 0–100 spectrum.

A fully interactive Flask website allows users to play Wavelength games directly against Wally.

## Setup

**Clone Repository:**
```bash
git clone https://github.com/Akigaii/wally
cd wally
```

**Install Dependencies:**
```bash
pip install -r requirements.txt
```

**Run App:**
```bash
python app.py
```

Then open your browser and go to `http://localhost:5000`.

## How to Play

1. Draw a word pair (e.g., Hot / Cold)
2. Enter a clue word or phrase (e.g., "lava")
3. Wally will predict where the needle should land on the spectrum
4. Compare Wally's guess to the hidden value and see how many points it scores

## Project Structure

```
wally/
├── app.py              # Flask application
├── model/              # Fine-tuned model weights
├── history/            # Experiment JSON history files
├── graphs/             # Generated experiment graphs
├── templates/          # HTML templates
├── static/             # CSS, JS, assets
└── requirements.txt    # Python dependencies
```
