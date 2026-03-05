# Django Paginação (CBV + Bootstrap)

Projeto simples em **Django** criado com foco em **estudar paginação** usando **Class-Based Views (ListView)** e um template de paginação com **Bootstrap**. :contentReference[oaicite:0]{index=0}

---

## 🎯 Objetivo do projeto

- Praticar **paginação nativa do Django** com `ListView`
- Entender como o Django expõe no template:
  - `page_obj`
  - `paginator`
  - `is_paginated`
- Renderizar a navegação de páginas com **Bootstrap** (anterior/próxima + números) :contentReference[oaicite:1]{index=1}

---

## ✅ O que foi implementado

- Model simples `Produto` (`nome`, `preco`, `descricao`) :contentReference[oaicite:2]{index=2}
- Listagem paginada com `ListView` e `paginate_by = 2` :contentReference[oaicite:3]{index=3}
- Template `index.html` exibindo os itens com `page_obj` e incluindo o partial `paginacao.html` :contentReference[oaicite:4]{index=4}
- Partial `paginacao.html` com:
  - botão **«** / **»**
  - loop em `paginator.page_range`
  - página ativa destacada :contentReference[oaicite:5]{index=5}

---

## 🧰 Tecnologias

- Python
- Django **6.0.3** :contentReference[oaicite:6]{index=6}
- django-bootstrap4 :contentReference[oaicite:7]{index=7}

---

## 📁 Estrutura (resumo)

```bash
Django_paginacao/
├─ core/
│  ├─ models.py
│  ├─ views.py
│  ├─ urls.py
│  └─ templates/
│     ├─ index.html
│     └─ paginacao.html
├─ dpag/
│  ├─ settings.py
│  └─ urls.py
├─ manage.py
└─ requirements.txt