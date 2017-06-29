Based on Dockerfile from [Christian Meter](https://github.com/n2o)

# Install
``` bash
docker build -t dockerlatex .
```

# Start
``` bash
docker run -it --rm=true -v ~/Documents/Dissertation:/tex dockerlatex latexmk -pvc -bibtex -view=none -quiet -pdf thesis.tex
```

# Optional local IDE configuration
## Okular
``` bash
sudo apt-get install okular
```
## Sublime
https://www.sublimetext.com/docs/3/linux_repositories.html

Replace `~/.config/sublime-text-3/Packages/User/Preferences.sublime-settings` with the file from this directory
