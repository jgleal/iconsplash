# iconsplash
Generate icons and splash screens for apps
### Prerequisites
You need imagemagick and jp installed:
```sh
$ apt-get install imagemagick jp
```
### Config
The config.json file contains all for generate the resources. Change it if nececesary
```json
{
	"package": "PGB",
	"output": [{
		"category": "iOS icon",
		"description": "iOS icons",
		"path": "resources/ios/icon",
		"source": "icon.png",
		"sizes": [{
			"file": "icon-40.png",
			"width": 40,
			"height": 40
		}, {
			"file": "icon-40@2x.png",
			"width": 80,
			"height": 80
		}, {
			"....": "....",
			"....": "...."
		}]
	}, {
		"category": "iOS_landscape",
		"description": "iOS landscape splashscreens",
		"path": "resources/ios/splash",
		"source": "screen_land.png",
		"sizes": ["..."]
	}]
}
```
### Use
It's a simply bash script, you don't need install anymore:
```sh
$ ./iconsplash
```