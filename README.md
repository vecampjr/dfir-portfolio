mkdir dfir-portfolio
cd dfir-portfolio

git init -b main

for d in 01-acquisition 02-disk-analysis 03-mobile 04-scripts; do
  mkdir "$d"
  echo "# $d" > "$d/README.md"
done

echo "# DFIR Portfolio" > README.md

git add .
git commit -m "Initial structure"
