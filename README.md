# Django Blog

A simple blog web application built with Django, featuring post creation, editing, deletion, and viewing capabilities. It includes a user-friendly interface and an admin panel for content management.

## Features
- Create, read, update, and delete (CRUD) blog posts
- Admin interface for managing content
- Responsive design with Bootstrap
- Custom CSS styling for a clean look

## Installation

### Prerequisites
- Python 3.8 or higher
- Django 5.2.6
- Virtual environment (recommended)

### Tech Stack

Backend: Django 5.2.6, Python 3.12.7
Frontend: Bootstrap 5.3.0, HTML, CSS
Database: SQLite (development environment)
Static Files: Django static files


# Project Structure
```
djblog/                     # root
├── blog/                   # APP(*)
│   ├── migrations/         
│   ├── templates/       
│   │   ├── blog/          
│   │   ├── base.html      
│   ├── static/            # STATICS (css, js..)
│   │   ├── css/
│   │   │   ├── style.css
│   ├── __init__.py
│   ├── admin.py           
│   ├── apps.py            
│   ├── forms.py           
│   ├── models.py          # db models
│   ├── urls.py            # URL routing
│   ├── views.py           # view logic
│ 
├── myblog/                # SETTING(*)
│   ├── __init__.py
│   ├── settings.py        # 프로젝트 설정 (DB, 앱, 템플릿 등)
│   ├── urls.py            # 프로젝트 전체 URL 라우팅
│   ├── wsgi.py            # 배포용 WSGI 설정
├── static/                # 프로젝트 수준 정적 파일
├── manage.py              # 장고 관리 명령어 스크립트
├── requirements.txt       # 의존성 목록
├── .gitignore             # 깃 제외 파일
├── README.md              # 프로젝트 설명

```



## more about django
Django as a Backend Framework
MTV(model - template - view)


-manage db: define model structure(models.py) ORM(object-relational mapping; without SQL)
-request handling: vies.py, urls.py
-security: handles CSRF protection, user authentication, data validation
-business(server) logic


## about Migration
managing database schema changes, updating 'data blueprint(tables)' when you change the structure of your data(models)

-sync models with database: models.py define the structure of database tables
-track changes: this allows you to update the database w/o losing data or manually writing SQL
-version control: like git for you db, letting you apply,revert, or track schema changes.