# OpnForm

<p align="center">
<img src="https://github.com/JhumanJ/OpnForm/blob/main/public/img/social-preview.png?raw=true">
</p>

<a href="https://github.com/jhumanj/OpnForm/actions"><img src="https://github.com/jhumanj/laravel-vue-tailwind-spa/workflows/tests/badge.svg" alt="Build Status"></a>

> An open-source form builder. It's an alternative to products like Typeform, JotForm, Tally etc.

## Features

- No-code form builder, with infinite number of fields & submissions
- Text inputs, Date inputs, URL inputs, Phone inputs, Email inputs, Checkboxes, Select and Multi-Select inputs, Number Inputs, Star-ratings, File uploads & more 
- Embed anywhere (on your website, in your Notion page, etc)
- Email notifications (for both form owner & form respondents)
- Hidden fields
- Form passwords
- URL form pre-fill
- Slack integration
- Webhooks
- Form logic
- Customize colors, add images or even some custom code
- Captcha form protection
- Form closing date
- Limit the number of submissions allowed

And much more!

## Getting started with OpnForm

The easiest way to get started with OpnForm is with the [official managed service in the Cloud](https://opnform.com/).

It takes 1 minute to try out the builder for free. You'll have high availability, backups, security, and maintenance all managed for you.

## Running the project locally

The project can be run locally via docker:
- Clone the project
- `cd` in the project
- Create a `.env` file with `mv .env.example .env`
- Start the docker container: `docker compose up -d`
- Get into the container's shell with `docker compose exec -it opnform-laravel.test-1 bash`
- Run the following commands. 
  - Run `npm install && npm run production`
  - Run `php artisan key:generate`
  - Run `php artisan jwt:secret`
  - Run `php artisan migrate`

You should now be able to access the application at [http://0.0.0.0:3000/](http://0.0.0.0:3000/). You can also access the file storage app Minio at [http://localhost:8900/](http://localhost:8900/) (default user: `sail`, default password: `secret`) and Mailhog, our email interceptor tool at [http://localhost:8025](http://localhost:8025)

## Self-hosting

This section hasn't been written yet, we need to work on this. 

## Tech Stack

OpnForm is a standard web application built with:
- [Laravel](https://laravel.com/) PHP framework
- [Vue.js](https://vuejs.org/) front-end framework
- [TailwindCSS](https://tailwindcss.com/)

## Contribute
You're more than welcome to contribute to this project. We don't have guidelines on this yet, but we will soon. In the meantime, feel free to ask [any question here](https://github.com/JhumanJ/OpnForm/discussions).

## License
OpnForm is open-source under the GNU Affero General Public License Version 3 (AGPLv3) or any later version. You can find it [here](https://github.com/JhumanJ/OpnForm/blob/main/LICENSE).

