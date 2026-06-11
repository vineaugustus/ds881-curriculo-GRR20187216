# Currículo Online — DS881

![CI/CD](https://github.com/vineaugustus/ds881-curriculo-GRR20187216/actions/workflows/main.yml/badge.svg)

## 🔗 Site em produção

[Acesse o currículo aqui](https://vineaugustus.github.io/ds881-curriculo-GRR20187216/)

---

## 🐳 Como executar localmente com Docker

### Pré-requisitos
- [Docker](https://www.docker.com/) instalado
- [Docker Compose](https://docs.docker.com/compose/) instalado

### Passos

1. Clone o repositório:
```bash
   git clone https://github.com/vineaugustus/ds881-curriculo-GRR20187216.git
   cd ds881-curriculo-GRR20187216
```

2. Suba o container:
```bash
   docker compose up
```

4. Para parar o container:
```bash
   docker compose down
```

---

## 🔒 Proteção da branch `main`

A branch `main` está protegida com as seguintes regras:

- Push direto bloqueado — toda alteração deve ser feita via Pull Request
- Merge só permitido com o CI verde (Linter HTML + Build passando)
- Force push bloqueado
- Deleção da branch bloqueada

---

## 📌 Fluxo de trabalho

```bash
# Criar nova branch
git checkout -b feat/nome-da-feature

# Após as alterações, commitar seguindo Conventional Commits
git add .
git commit -m "feat: descrição da alteração"

# Enviar para o GitHub
git push origin feat/nome-da-feature

# Abrir Pull Request no GitHub e aguardar CI verde para fazer merge
```