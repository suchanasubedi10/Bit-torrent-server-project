[![progress-banner](https://backend.codecrafters.io/progress/bittorrent/5c8f5ea0-b461-4de0-a074-e4c9f5b5ab28)](https://app.codecrafters.io/users/codecrafters-bot?r=2qF)

In this challenge, you’ll build a BitTorrent client that's capable of parsing a
.torrent file and downloading a file from a peer. Along the way, we’ll learn
about how torrent files are structured, HTTP trackers, BitTorrent’s Peer
Protocol, pipelining and more.

# 1. Torrent File Information:

##### Navigate to the `app` directory and run the following command. Make sure that your `main.py` and `sample.torrent` should be in the same directory.

```sh
python main.py info sample.torrent
```

## 2. Torrent File Information:

```sh
python main.py peers sample.torrent
```

# 3. Handshake with Peer:

```sh
python main.py handshake sample.torrent "your_any_one_peers_sample"  //for_example: 192.168.1.5:6881"
```

## 4. Download a Specific Piece:

```sh
python main.py download_piece -o piece1.dat sample.torrent 0
```

## 5. Download Entire Torrent:

```sh
python main.py download -o complete_file.dat sample.torrent

```
