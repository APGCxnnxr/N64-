# Nintendo 32 - Web N64 Emulator

Nintendo N64 displayed in a browser window and controlled by a smartphone. Emscripten compiled mupen64plus, ionic app, socket.io input proxying, and a paradrop chute wrapper.

You need to bring your own ROM to play, or choose one from the list to download. ( IDC about Nintendo ) 

Chrome has issues rendering the display. IDK how to fix it.  Please use firefox if you encounter problems.

To simplify the running locally by yourself, make a new codespace of the forked repository, do npm install, then once its finished, to npm start.
then go to the port. ( You Dont have to make it public ) 

This stuff below is left over stuff incase you know wat your doing.

## Running

Running locally:

```
npm install
npm start 
```

Go to [localhost:3000/](http://localhost:3000) in your browser and [localhost:3000/controller](http://localhost:3000/controller) on phone. 

To run on a paradrop router:

- Install the chute from [paradrop.org](http://paradrop.org) on your already provisioned router. The chute is called `nintendo64`.
- Connect to the router's WiFi
- Go to [192.168.1.1:3000](http://192.168.1.1:3000) in your browser
- Go to [192.168.1.1:3000/controller](http://192.168.1.1:3000/controller) on your smartphone

## To Do

- Multiplayer
- Canvas Streaming 
- Lobbies


## References

Credit where credit is due-- almost all of this is taken off-the-shelf. These repos made up most of the code found here:

- [mupen64plus](https://github.com/mupen64plus) 
- [jquesnelle's emscripten project](https://github.com/jquesnelle/mupen64plus-ui-console/tree/emscripten)
- [webvr polyfill](https://github.com/googlevr/webvr-polyfill)
