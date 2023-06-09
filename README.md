# Directus On Railway

This example deploys a self-hosted version of [Directus](https://directus.io).

Internally it uses an external PostgreSQL database (Supabase) to store the data and S3 to store files.

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template/directus-supabase?referralCode=wassim)

## ✨ Features

- Directus
- Postgres
- Supabase
- S3
- Slugs (via inclusion of [https://github.com/dimitrov-adrian/directus-extension-wpslug-interface](https://github.com/dimitrov-adrian/directus-extension-wpslug-interface))

## 💁‍♀️ How to use

- Click the Railway button 👆
- Add the environment variables
  - If you do not add the S3 related environment variables, your images/files will not be persisted between deploys.

## 📝 Notes

- After your app is deployed, visit the `/admin` endpoint to login using the initial admin user you entered during config.
- Railway's filesystem is ephemeral which is why any changes to the filesystem are not persisted between deploys. This is why, this example uses S3 for storage.

## Credit

Originally forked from [https://github.com/azrikahar/directus-railway-starter](https://github.com/azrikahar/directus-railway-starter) with Supabase, S3 and Slugs support built in off the bat.
