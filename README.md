# VSCabbage React example

This example will show you how to synchronize a [Cabbage](https://cabbageaudio.com/) project with a [React](https://github.com/facebook/react) using [vscabbage-react](https://github.com/hdale94/vscabbage-react).

The React project is built with Vite and TypeScript.

There are examples of functional components (sliders) that implement the useCabbageState hook to get and set the channel values.

## Steps to replace Cabbage UI with React build

### 1. Export the Example.csd file to VST3 effect.

### 2. Move the exported VST3 file into a recognized folder of your host.

#### Windows:

    C:/Program Files/Common Files/VST3

### 3. Run the “Build project” command in the "react"-folder.

### 4. Move the build (files in the dist-folder) into:

    C:/ProgramData/CabbageAudio/Example

### 5. Load plugin in your host, and the plugin UI should be the React build.

## Commands

### Run project:

    yarn run dev

### Build project:

    yarn build

### Copy build into plugin folder

    cp ./dist/* C:/ProgramData/CabbageAudio/PluginName -Recurse -Force
