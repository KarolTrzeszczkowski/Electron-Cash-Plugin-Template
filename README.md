# Electron Cash Plugin Template

This project is a template that may serve as a foundation for new plugins for Electron Cash BCH wallet. 
It does exactly nothing, but registers itself in Electron Cash and unregisters. You can fill it with any functionality you like
and add it to your wallet.

This template is basically [EC Scheduled Payment Plugin](https://github.com/rt121212121/electron_cash_scheduled_payments_plugin) 
by Roger Taylor, stripped from everything that makes any sense. 

## Renaming the plugin
Enter the directory where you unpacked the plugin and execute commands:

```cp -r Electron-Cash-Plugin-Template-master/ my-plugin-name/; cd my-plugin-name```

```sed -i s/template/my-plugin-name/g manifest.json```

```sed -i s/template/my-plugin-name/g template/*```

```sed -i s/Template/'My Plugin Name'/g manifest.json```

```sed -i s/Template/'My Plugin Name'/g template/*```

```mv template my-plugin-name```

You can do it "by hand" as well, just enter every file and change the name everywhere you see it. I recommend it if you are making your first plugin.

## Packing the plugin
To pack your plugin execute:
```zip -r my-plugin-name manifest.json my-plugin-name/```
Or simply select ```manifest.json``` and ```my-plugin-name/``` file, right-click and create a zip archive. 

