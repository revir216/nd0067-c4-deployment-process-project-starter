# Dependencies

```
- Node v14.15.1 (LTS) or more recent. 

- npm 6.14.8 (LTS) or more recent.

- AWS CLI v2, v1 can work but was not tested for this project

- AWS RDS for PostgreSQL database. Preferred version is 14.x.

- AWS S3 bucket for hosting front-end files.

```

## Setup Back-end Application

### Open Git Bash or Terminal.

source set_env.sh

cd udagram-api/

### Install the package dependencies, and ignore the warnings
npm install .
### Generate the "www/" folder contaning the autogenerated files.
npx tsc

npm run start
### If everything works fine with the "npm run start"
npm run dev

## Setup Front-end Application

### Open Git Bash or Terminal.
source set_env.sh
cd udagram-frontend/

### Install the package dependencies FORCEFULLY, and ignore the warnings
npm install -f
### Build your application by compiling it into static files
ionic build
### Run the application locally
ionic serve