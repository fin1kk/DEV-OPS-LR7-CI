# DEV-OPS-LR6-CI (Ansible + CI/CD Integration)
Данный проект демонстрирует добавление функций **CI/CD** для автоматической проверки и выполнения Ansible-плейбуков с помощью **GitHub Actions**.  
Репозиторий основан на предыдущей лабораторной работе (деплой nginx с использованием роли Ansible).

## Содержимое репозитория
 - 6lr_playbook.yml — основной Ansible-плейбук для деплоя nginx с vhosts.
 - roles/nginx-vhosts/ — роль для установки и настройки nginx.
 - run_playbook.sh — вспомогательный скрипт для запуска плейбука вручную.
 - .github/workflows/ci.yml — файл CI-пайплайна GitHub Actions.

## Используемые технологии
 - Ansible — автоматизация конфигурации и деплоя.
 - GitHub Actions / GitLab CI — автоматизация процессов CI/CD.
 - nginx — веб-сервер для тестового деплоя.

## Результат
После каждого push или pull request пайплайн:
 - автоматически проверяет синтаксис и структуру плейбука;
 - выводит результат проверки в GitHub Actions (или GitLab CI) интерфейсе;
 - при необходимости может быть расширен для тестового деплоя на виртуальной машине.

## Скриншоты
<img width="1246" height="636" alt="image" src="https://github.com/user-attachments/assets/ed1015a4-1637-47af-87ae-e069c5bcee22" />

После изменений:
<img width="1280" height="291" alt="image" src="https://github.com/user-attachments/assets/81a99f7e-8507-47f9-9252-08aa45c48317" />
