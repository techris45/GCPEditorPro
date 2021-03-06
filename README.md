# GCP Editor Pro

Amazingly Fast and Simple Ground Control Points Interface for [OpenDroneMap](https://opendronemap.org) software.

![image](https://user-images.githubusercontent.com/1951843/80494281-7e63dd00-8934-11ea-9176-75e37db5bb97.png)

## Features

- Import GPS measurements from CSV
- Easy/fast image selection
- Create GCPs from scratch by clicking on a map
- Custom basemap selector
- Geocoder
- Import existing GCP Files
- Offline capable
- Cross platform (Windows, Mac, Linux, Web)
- WebODM Integration (Plugin)

## Installation

The easiest, most convenient way to run the software is to [download the prebuilt releases](https://uav4geo.com/software/gcpeditorpro), which can be downloaded freely for evaluation. 

You will need to [purchase a license](https://uav4geo.com/software/gcpeditorpro#buy) to unlock the prebuild releases after evaluation. Your purchase helps support the development of the software ❤

If you don't want to pay for a license, you can compile the software from sources (see instructions below). If you choose to compile from sources, you are free to use, copy, distribute and modify the software, provided that you are the **only** user of the software. See the terms of the [Fair Source License](https://github.com/uav4geo/GCPEditorPro/blob/master/LICENSE) for details.

## Compile From Sources

The application is written using [Angular](https://angular.io).

You will need to install:
 * [NodeJS](https://nodejs.org/en/)
 
Extract the source code in a directory, then from the directory:

```bash
npm install
ng serve
```

After a while, the application should be available from your browser at http://localhost:4200.

You can build the electron apps and the WebODM plugin by running:

```bash
# Windows
dist.bat

# Linux/Mac
./dist.sh
```

But note that you'll need to modify the storage service (around https://github.com/uav4geo/GCPEditorPro/blob/master/src/app/storage.service.ts#L53) to return a `DevLicense` if you want to remove the licensing dialogs.

Results will be stored in the `dist/` folder.

You can run `npm run stats` to analyze production bundle size

## Contributing

We welcome contributions to improve GCP Editor Pro. If you want to add something, please open a pull request. Please note that the copyright of any contribution will have to be gifted to UAV4GEO because of the [Fair Source License](https://github.com/uav4geo/GCPEditorPro/blob/master/LICENSE).

## Reporting Issues

Please [open an issue](https://github.com/uav4geo/GCPEditorPro/issues) if you find a problem with the software.

## FAQ

### How is the Fair Source License similar to (or different from) open-source licenses?

The Fair Source License is not an open-source license and doesn’t intend to be an open-source license. Fair Source allows usage, redistribution, and modification when the usage is below the Use Limitation. Once an organization exceeds the Use Limitation (which is determined by the licensor), it must pay a license fee to continue doing those things.

### If I modify the source code, can I redistribute my modified version under the MIT License?

No. Your modified version consists of the original software (which is under the Fair Source License) and your modifications, which together constitute a derivative work of the original software. The license does not grant you the right to redistribute under a license like MIT without the Use Limitation.





