FROM uochan/antq AS BASE

LABEL "com.github.actions.name"="Leiningen Dependency Update Action"
LABEL "com.github.actions.description"="A simple GitHub Actions to create Pull Requests for outdated leiningen dependencies"
LABEL "com.github.actions.color"="purple"
LABEL "com.github.actions.icon"="git-pull-request"

LABEL "repository"="https://github.com/nnichols/leiningen-dependency-update-action"
LABEL "homepage"="https://github.com/nnichols"
LABEL "maintainer"="Nick Nichols <nichols1991@gmail.com>"
LABEL "version"="v1.0.0"

RUN apt update -y
RUN apt install --no-install-recommends -y gnupg2 software-properties-common
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key C99B11DEB97541F0
RUN apt-add-repository https://cli.github.com/packages
RUN apt update -y
RUN apt install -y gh git
