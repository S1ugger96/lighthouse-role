# LightHouse Role

Роль для загрузки веб-интерфейса LightHouse для ClickHouse.

### Что делает роль:
- Устанавливает git
- Создает директорию для веб-страниц (`/var/www/lighthouse`)
- Клонирует исходники LightHouse

### Переменные по умолчанию (`defaults/main.yml`):
- `lighthouse_version: "master"` — ветка или тег репозитория
- `lighthouse_repo_url: "https://github.com/VKCOM/lighthouse.git"` — URL репозитория
- `lighthouse_install_dir: "/var/www/lighthouse"` — директория установки

### Пример вызова:
```yaml
- hosts: all
  roles:
    - lighthouse-role
