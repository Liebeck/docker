Based on Dockerfile from [Christian Meter](https://github.com/n2o)

# Install
docker build -t dockerlatex .

# Start
docker run -it --rm=true -v ~/Documents/Dissertation:/tex dockerlatex latexmk -pvc -bibtex -view=none -quiet -pdf thesis.tex


# Optional local IDE configuration
## Okular
``` bash
sudo apt-get install okular
```
## Sublime
``` bash
sudo apt-get install sublime-text
```

Replace `~/.config/sublime-text-3/Packages/User/Preferences.sublime-settings` with the file from this directory