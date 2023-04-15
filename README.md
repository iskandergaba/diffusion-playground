# Diffusion Models Playground

## Set up the Environment
To get started, create the time series environment using:
```bash
conda env create -f environment.yml
```

## Save Environment
If you update a package, remove or add other packages during your experimentation, you can save your updated environment using the command below for easier replication:
```bash
conda env export --no-builds | grep -v "^prefix: " > environment.yml
```

## Remove Environment
- You can remove the environment using the following command:
```bash
conda remove -n diffusion-playground
```
- If you want to remove the installed packages from Conda as well, add `--all` flag at the end of the command:
```bash
conda remove -n diffusion-playground --all
```