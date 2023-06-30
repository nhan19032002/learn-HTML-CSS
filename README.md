## Set up

**Trước tiên, bạn cần phỉa cài đặt [NodeJS](https://nodejs.org/), [Yarn](https://yarnpkg.com/)**

Sau đó làm theo các bước:

#### Step 1:

` git clone https://github.com/SiVi-Code/source-market-be.git` - Clone dự án

#### Step 2: 

`cd source-market-be` - Truy cập project files

#### Step 3: 

`yarn` (or `npm install`) - install dependencies

#### Step 4:

Tạo file `.env` ở thư mục gốc của dự án và thêm

```
# ===============================
# = GENERAL
# ===============================
PORT=8000
NODE_ENV=dev
JWT_SECRET=test
JWT_EXPIRES_IN_HOUR=24h

CLIENT_URL=http://localhost:8080
SERVER_URL=http://localhost:3000
SWAGGER_URL=http://localhost:3000/api/v1

# ===============================
# = DATABASE MYSQL
# ===============================
DB_HOST_MYSQL=db4free.net
DB_PORT_MYSQL=3306
DB_USERNAME_MYSQL=db_sellsource
DB_NAME_MYSQL=db_sellsource
DB_PASSWORD_MYSQL=db_sellsource
DB_LOGGING=DISABLED

# ===============================
# = SEEDING
# ===============================
TYPEORM_SEEDING_FACTORIES=dist/database/factories/*.js
TYPEORM_SEEDING_SEEDS=dist/database/seeds/*.js

# ===============================
# = LOGGER
# ===============================
LOGGER_CONSOLE_SILENT=true
LOGGER_MAX_SIZE_SILENT=false
LOGGER_MAX_SIZE_PATH=logs/logs_size/logs.log
LOGGER_DAILY_SILENT=false
LOGGER_DAILY_PATH=logs/logs_daily/logs-%DATE%.log
LOGGER_DAILY_PATTERN=YYYY-MM-DD-HH

# ===============================
# = GOOGLE
# ===============================
GOOGLE_CLIENT_ID=978594913614-d38725tm2i7djnkslpo6om6rujkt4js9.apps.googleusercontent.com
GOOGLE_SECRET=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

# ===============================
# = CORS
# ===============================
CORS_ALLOWED_URL=https://source-market-api-im6m.onrender.com,https://source-market-call-api-from-local.onrender.com,http://localhost:3000,http://localhost:8080

# ===============================
# = FACEBOOK
# ===============================
FACEBOOK_CLIENT_ID=2815325912026613
FACEBOOK_SECRET=69a4710b2367c51fe592c58e3c83e829
```
