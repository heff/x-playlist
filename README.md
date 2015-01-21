# &lt;x-playlist&gt;

> A simple [web component](http://webcomponents.org) [custom element](http://w3c.github.io/webcomponents/spec/custom/) for playing through a list of video and/or audio elements.

## Demo

[Check it live!](http://heff.github.io/x-playlist)

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install x-playlist --save
```

Or [download as ZIP](https://github.com/heff/x-playlist/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="bower_components/webcomponentsjs/webcomponents.min.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="bower_components/x-playlist/src/x-playlist.html">
    ```

3. Start using it!

    ```html
    <x-playlist>
        <video src="my_video_1.mp4" controls preload="none">
        <video src="my_video_2.mp4" controls preload="none">
        <audio src="my_audio_1.mp3" controls preload="none">
    </x-playlist>
    ```

## Options

Attribute     | Options     | Default      | Description
---           | ---         | ---          | ---
`loop`        | *boolean*   | `false`      | Loop back to the first media at the end

## Methods

Method        | Parameters   | Returns     | Description
---           | ---          | ---         | ---
`previous()`  | None.        | Nothing.    | Play the previous media element
`next()`      | None.        | Nothing.    | Play the next media element

## Development

In order to run it locally you'll need to fetch some dependencies and a basic server setup.

* Install [Bower](http://bower.io/) & [Grunt](http://gruntjs.com/):

    ```sh
    $ [sudo] npm install -g bower grunt-cli
    ```

* Install local dependencies:

    ```sh
    $ bower install && npm install
    ```

* To test your project, start the development server and open `http://localhost:8000`.

    ```sh
    $ grunt server
    ```

* To provide a live demo, send everything to `gh-pages` branch.

    ```sh
    $ grunt deploy
    ```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

For detailed changelog, check [Releases](https://github.com/heff/x-playlist/releases).

## License

[MIT License](http://opensource.org/licenses/MIT)
