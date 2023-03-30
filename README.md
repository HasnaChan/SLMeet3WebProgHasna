<p align="center"><a href="https://github.com/HasnaChan/SLMeet3WebProgHasna" target="_blank">Hi, I am Hasna.</a></p>

## About this Project
My name is Hasna Salsabilla Abdullah. This website made with PHP Framework Laravel. The design inspired by Bootstrap. Here is the interface of this website:


![1. Home Page](https://github.com/HasnaChan/SLMeet3WebProgHasna/blob/main/web%20documentation/home.jpg)
![2. About Me Page](https://github.com/HasnaChan/SLMeet3WebProgHasna/blob/main/web%20documentation/about.jpg)
![3. Resume Page](https://github.com/HasnaChan/SLMeet3WebProgHasna/blob/main/web%20documentation/resume.jpg)
![4. Project Page](https://github.com/HasnaChan/SLMeet3WebProgHasna/blob/main/web%20documentation/resume.jpg)
![5. Blog Page](https://github.com/HasnaChan/SLMeet3WebProgHasna/blob/main/web%20documentation/blog.jpg)

**Steps I did to install NPM Bootstrap:**

**Step 1:** Download and install Node.js 

**Step 2:** Install Laravel Project
   ```
   composer global require laravel/installer
   ```
   
**Step 3:** Make new project
   ```
   laravel new SLMeet3Hasna
   ```
   
**Step 4:** Install Laravel UI For Bootstrap 5
   ```
   composer require laravel/ui
   ```
   
**Step 5:** Setup Auth Scaffolding with Bootstrap 5
   ```
   php artisan ui bootstrap --auth
   ```
   
**Step 6:** Setup Auth Scaffolding with Bootstrap 5
   ```
   php artisan ui bootstrap --auth
   ```
   
**Step7:** Install NPM Dependencies
   ```
   npm install
   ```
**Step 8:** Import vite.config.js Bootstrap 5 Path
   ```
    import { defineConfig } from 'vite';
    import laravel from 'laravel-vite-plugin';
    import path from 'path'

    export default defineConfig({
        plugins: [
            laravel([
                'resources/js/app.js',
            ]),
        ],
        resolve: {
            alias: {
                '~bootstrap': path.resolve(__dirname, 'node_modules/bootstrap'),
            }
        },
    });

   ```

**Step 9:** Update bootstrap.js
   ```
       import loadash from 'lodash'
    window._ = loadash


    import * as Popper from '@popperjs/core'
    window.Popper = Popper

    import 'bootstrap'

    import axios from 'axios'
    window.axios = axios

    window.axios.defaults.headers.common['X-Requested-With'] = 'XMLHttpRequest';
   ```

**Step 10:** Import Bootstrap 5 SCSS in JS Folder
   ```
   import './bootstrap';

    import '../sass/app.scss'
   ```
**Step 11:** Replace mix() with @vite Blade directive
   ```
   @vite(['resources/js/app.js'])
   ```

**Step 12:** Running Vite Command to build Asset File
   ```
   npm run build
   ```

**Step 12:** Start the Local server
   ```
   php artisan serve
   ```
   
   
## License
https://getbootstrap.com/docs/5.0/getting-started/introduction/
https://www.google.com/search?q=bootstrapmade&oq=bo&aqs=chrome.0.69i59l4j69i60l4.1101j0j7&sourceid=chrome&ie=UTF-8
