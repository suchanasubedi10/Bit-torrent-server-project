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

**Expected output**:

##### Should include tracker URL, length, info hash, piece length, and piece hashes.

```sh
Tracker URL: http://bittorrent-test-tracker.codecrafters.io/announce
Length: 92063
Info Hash: d69f91e6b2ae4c542468d1073a71d4ea13879a7f
Piece Length: 32768
Piece Hashes:
e876f67a2a8886e8f36b136726c30fa29703022d
6e2275e604a0766656736e81ff10b55204ad8d35
f00d937a0213df1982bc8d097227ad9e909acc17
```

## 2. Torrent File Information:

```sh
python main.py peers sample.torrent
```

**Expected output**:

##### List of peers in IP

```sh
165.232.33.77:51498
178.62.82.89:51448
178.62.85.20:51489
```

## 3. Handshake with Peer:

```sh
python main.py handshake sample.torrent "your_any_one_peers_sample"  `for_example: 178.62.82.89:51448`
```

**Expected output**:

```sh
Peer ID: 2d524e302e302e302d71436ef031d3d90fc6cb18
```

## 4. Download a Specific Piece:

```sh
python main.py download_piece -o piece1.dat sample.torrent 0
```

## 5. Download Entire Torrent:

```sh
python main.py download -o complete_file.dat sample.torrent

```
