mkdir new-project  
cd new-project  
git init  
cat "init" > README.md  
git add README.md  
git commit -m "init"
# наступна команда використовується для перейменування поточної гілки в Git.
git branch -M main 
# Створюємо нову гілку та переходимо до неї:
git checkout -b development
nano README.md
git add .
git commit -m "Add instruction to README.md"
# Повертаємось на основну гілку 
git checkout main
# Об'єднуємо зміни з гілки "development" у гілку "main" в репозиторії Git
git merge development
# Підключаємо віддалений репозиторій: 
git remote add origin https://github.com/vit-um/new-project.git
# Заливаємо в нього дані
git push
