# SymRs

Fork of SymPy progressively rewritten in Rust.

## Installation
```
conda create --name symrs python=3.12
conda activate symrs
pip install -r requirements-dev.txt 
(cd rust_extension && maturin build && pip install target/wheels/rust_extension*.whl)
python -c "import rust_extension; print(rust_extension.sum_as_string(1, 2))"
```

## Development
```
(cd rust_extension && maturin develop)
```