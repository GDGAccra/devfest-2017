### Features
  - [x] Polymer
  - [x] [PRPL pattern](https://www.polymer-project.org/1.0/toolbox/server)
  - [x] Offline access
  - [x] Material design
  - [x] Animations
  - [x] Integrated speakers and sessions management
  - [x] SEO friendly
  - [x] Optimized and fast
  - [x] Editable theme colors
  - [x] Quick deploy (with [Travis CI](/docs/tutorials/deploy.md))
  - [x] My schedule
  - [x] Firebase Data Loading :new:
  - [x] Sessions star rating :new:

### Setup
:book: [Full documentation](/docs/).

##### Docker-based development environment

If you don't want to bother with the dependencies, you can use the docker container for development.

Build the docker image:

    docker build -t devfest .

and execute the commands associated to the docker env in the following documentation:

:book: Read more in [docker docs](/docs/tutorials/docker.md).

:point_right: **[Fork](https://github.com/GDGGhana/devfest-2017/fork) this repository** and clone it locally.

##### Install dependencies

    npm install

Or you can install with Docker container:

    docker run -v "$PWD":/app devfest npm install

##### Start the development server

This command serves the app at `http://localhost:3000` and provides basic URL
routing for the app:

    npm run serve

Or you can serve Docker container:

    docker run -v "$PWD":/app devfest 

:book: Read more in [setup docs](/docs/tutorials/set-up.md).


### Build

This command performs HTML, CSS, and JS minification on the application
dependencies, and generates a service-worker.js file with code to pre-cache the
dependencies based on the entrypoint and fragments specified in `polymer.json`.
The minified files are output to the `build`.

    npm run build

Or you can build in Docker container:

    docker run -v "$PWD":/app devfest npm run build

:book: Read more in [deploy docs](/docs/tutorials/deploy.md).

### Contributing

##### General workflow
1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Make your changes
4. Run the tests, adding new ones for your code if necessary
5. Commit your changes (`git commit -am 'Added some feature'`)
6. Push to the branch (`git push origin my-new-feature`)
7. Create new Pull Request

:book: Read complete [contributing guide](CONTRIBUTING.md).


###### The GDG App, GDG[x] are not endorsed and/or supported by Google, the corporation.


### License

This is a hoverboard fork so inherits its license, and every other stuff

Project is published under the [MIT license](https://github.com/gdg-x/hoverboard/blob/master/LICENSE.md).
Feel free to clone and modify repo as you want, but don't forget to add reference to authors :)
