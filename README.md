# =========================================
# CRIAR PROJETO EQUIDADEIA NO GITHUB
# =========================================

# 1. Criar pasta do projeto
mkdir equidadeia

# 2. Entrar na pasta
cd equidadeia

# =========================================
# INICIAR GIT
# =========================================

git init

# =========================================
# CRIAR FRONTEND WEB
# =========================================

npm create vite@latest frontend-web -- --template react

# =========================================
# CRIAR BACKEND
# =========================================

mkdir backend

cd backend

npm init -y

npm install express cors dotenv openai firebase-admin axios

npm install nodemon --save-dev

cd ..

# =========================================
# CRIAR MOBILE APP
# =========================================

npx create-expo-app mobile

# =========================================
# CRIAR ESTRUTURA
# =========================================

mkdir docs

touch README.md
touch .gitignore

# =========================================
# .GITIGNORE
# =========================================

echo "node_modules/
.env
dist/
.firebase/
.expo/
.vscode/" > .gitignore

# =========================================
# PRIMEIRO COMMIT
# =========================================

git add .

git commit -m "Projeto inicial EquidadeIA"

# =========================================
# CONECTAR AO GITHUB
# =========================================

git remote add origin https://github.com/SEU-USUARIO/equidadeia.git

git branch -M main

git push -u origin main

