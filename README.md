# notes

find . -maxdepth 3 -type f \
  \( -iname '*readme*' -o -iname '*test*' \
  -o -name 'requirements*.txt' -o -name 'pyproject.toml' \
  -o -name 'package.json' -o -name 'Makefile' \
  -o -name 'Dockerfile' -o -name '*compose*.yml' \
  -o -name '*compose*.yaml' \) \
  -not -path './.git/*'
