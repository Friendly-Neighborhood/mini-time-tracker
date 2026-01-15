🚀 MINI-TIME-TRACKER — How to Run (from ZIP)
✅ Requirements

Убедитесь что установлено:

Node.js 18+

npm

1) Unzip project

Распакуйте архив и откройте папку проекта:

cd MINI-TIME-TRACKER

2) Install dependencies
Backend (API)
cd apps/api
npm install

Frontend (Web)
cd ../web
npm install

3) Setup database (Prisma + SQLite)

БД работает на SQLite, файл базы лежит внутри проекта:

apps/api/prisma/dev.db


Применяем миграции и генерируем Prisma client:

cd apps/api
npx prisma generate
npx prisma migrate dev

4) Run backend (API)
cd apps/api
npm run start:dev


✅ Backend запустится по адресу:
http://localhost:3001

5) Run frontend (Web)

Открыть второй терминал и выполнить:

cd apps/web
npm run dev


✅ Frontend будет доступен:
http://localhost:3000

✅ App usage

Открыть http://localhost:3000

Заполнить Time Entry Form

Нажать Save

Внизу отобразится история записей + суммы часов