# Vision to Language Navigation

A prefix-tuning approach to maze solving: a ResNet image encoder feeds a GPT-2 decoder,
which outputs the solution path as a sequence of moves (`U`, `D`, `L`, `R`).

## Contents

- `generate_dataset.py`, `generate_data.py`: create grid mazes where a given path is the only valid solution
- `image_duplication_check.ipynb`: detects duplicate maze images in a generated dataset
- `Untitled*.ipynb`: model experiments, result analysis and path-overlay visualisations
- `generated_sequences_*.json`, `detailed_results.json`: model outputs and evaluation results
- `*.png`: sample mazes, predictions and the model architecture diagram
- `ee641_report.pdf`: project report

## Generating data

```bash
python generate_dataset.py --size=4 --variations=150
```
