Онлайн-магазин книг

Це повноцінний вебдодаток для онлайн-магазину книг, створений з використанням Java (Spring Boot) для бекенду та React.js для фронтенду. Проєкт реалізовано в рамках навчального курсу зі стандартизації та документації програмних систем.

Проєкт використовує такі основні технології:

Бекенд реалізовано на Java 17 з використанням Spring Boot. Використовуються Spring Web, Spring Data JPA, PostgreSQL, Swagger для автоматичної генерації API-документації, а також Maven для управління залежностями.

Фронтенд реалізовано з використанням React.js, Tailwind CSS для стилізації, Axios для HTTP-запитів та react-router для маршрутизації. Також використовується компонент react-cookie-consent для реалізації GDPR cookie банеру.

Інші інструменти: Docker і Docker Compose для контейнеризації, GitHub для контролю версій, Storybook для демонстрації UI-компонентів, а також Docusaurus для документації системи.

Щоб запустити проєкт локально, необхідно:

1. Клонувати репозиторій:
git clone https://github.com/your-username/svoi-bookstore.git
cd svoi-bookstore

2. Запустити проєкт через Docker:
docker-compose up --build

Альтернативно можливо запустити бекенд і фронтенд окремо:

Для запуску бекенду:
cd backend
./mvnw spring-boot:run

Для запуску фронтенду:
cd frontend
npm install
npm start

Swagger доступний за адресою http://localhost:8080/swagger-ui/index.html

Storybook можна запустити командою:
cd frontend
npm run storybook

У проєкті реалізовано cookie banner згідно з вимогами GDPR. Користувач має можливість надати або відхилити згоду на обробку cookie.

Політика конфіденційності наведена у файлі PRIVACY_POLICY.md. У документі описано, які персональні дані збираються, як вони використовуються та які права має користувач згідно з GDPR.

Проєкт ліцензовано за умовами ліцензії MIT. Детальна інформація міститься у файлі LICENSE.md.

Розроблено в рамках курсу «Стандартизація та документація програмних систем». Автор: Легенький Костянти Миколайович ЗІПЗ-22-1. GitHub: github.com/your-username. 

Для перевірки ліцензійних залежностей можна скористатися такими командами:

npm install -g license-checker
license-checker --json > license-report.json

або

mvn project-info-reports:dependencies
