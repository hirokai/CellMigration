# Cell migration visualizer

## How to use

### Generate cell migration data

1. Run [find_cells-headless.fiji.py](https://gist.github.com/hirokai/142922ad9ecca053e540).
        * `/Applications/Fiji.app/Contents/MacOS/ImageJ-macosx --headless find_cells-headless.fiji.py /path/to/movie.avi`
        * This runs on Fiji in "headless mode"

    2. Run [calc_trajectories.py](https://gist.github.com/hirokai/eef5d08a1bd8e7c0e304)
    3. Put results (`hoge_coords.csv` and `hoge_connections_v2.csv`) in `data` folder.

### Prepare images of all frames

* Put in `img` folder.
* Base file name + '0000', '0001', etc.

### Edit `datasets` in `main.js`.

### Run server
`python -m SimpleHTTPServer`, and open [http://localhost:8000/](http://localhost:8000/).

## License

MIT license