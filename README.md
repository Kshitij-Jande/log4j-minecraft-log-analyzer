<br />
<div align="center">

  <h3 align="center" style="font-size: 2rem;">Log4j Minecraft Log Analyzer</h3>

  <p align="center">
    A very basic Python tool, that analyzes your Minecraft (client and server) log files, for specific strings, that could be used to locate previous attempts to exploit the Log4j vulnerability.
  </p>
</div>


## Libraries used

_Following are the libraries that have been used for this project._

- [Click](https://github.com/pallets/click)


## Getting Started

_Setting up this project should be easy._

1. Clone this repository.
```sh
git clone https://github.com/Kshitij-Jande/log4j-minecraft-log-analyzer.git
```
2. Install the necessary modules.
```sh
pip install -r requirements.txt
```
3. To locate your server logs, open your server's main folder, and copy the path to the `logs` folder.
4. If you don't know how to locate your logs folder, [click here](#locating-logs-folder).
5. Run the program, specifying the path to your server/client log folder.
```
python main.py --path (path-to-logs-folder)
```


## Locating `logs` folder

_Use the following to locate your `logs` folder._

- Server logs:
  1. Go to your server's main folder.
  2. Look for a folder named `logs`.
  3. Copy the path to this folder.
- Game logs (**Windows**):
  1. Hit `Windows + R` keys to open **Run**.
  2. Type `%appdata%` and hit enter.
  3. Go inside the `.minecraft` folder.
  4. Look for a folder named `logs`.
  5. Copy the path to this folder.
- Game logs (**macOS**):
  1. Hit `Command + Space` keys to open **Spotlight search**.
  2. Paste `~/Library/Application Support/minecraft/` and hit enter.
  3. If this is the correct path, you should be able to find the `logs` folder.
  4. The path to this folder should be `~/Library/Application Support/minecraft/logs/`.


## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
If you like this project, you can give it a star. Thanks.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature`)
3. Commit your Changes (`git commit -m 'Add some feature'`)
4. Push to the Branch (`git push origin feature`)
5. Open a Pull Request


## Acknowledgments

_Material that I used as a reference, to make this project._

- [Neo23x0's gist to detect Log4j RCE exploit](https://gist.github.com/Neo23x0/e4c8b03ff8cdf1fa63b7d15db6e3860b)