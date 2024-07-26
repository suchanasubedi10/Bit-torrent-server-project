[![progress-banner](https://backend.codecrafters.io/progress/bittorrent/5c8f5ea0-b461-4de0-a074-e4c9f5b5ab28)](https://app.codecrafters.io/users/codecrafters-bot?r=2qF)

This is a starting point for Python solutions to the
["Build Your Own BitTorrent" Challenge](https://app.codecrafters.io/courses/bittorrent/overview).

In this challenge, you’ll build a BitTorrent client that's capable of parsing a
.torrent file and downloading a file from a peer. Along the way, we’ll learn
about how torrent files are structured, HTTP trackers, BitTorrent’s Peer
Protocol, pipelining and more.

**Note**: If you're viewing this repo on GitHub, head over to
[codecrafters.io](https://codecrafters.io) to try the challenge.

# Passing the first stage

The entry point for your BitTorrent implementation is in `app/main.py`. Study
and uncomment the relevant code, and push your changes to pass the first stage:

```sh
git add .
git commit -m "pass 1st stage" # any msg
git push origin master
```

Time to move on to the next stage!

# Stage 2 & beyond

Note: This section is for stages 2 and beyond.

1. Ensure you have `python (3.11)` installed locally
1. Run `./your_bittorrent.sh` to run your program, which is implemented in
   `app/main.py`.
1. Commit your changes and run `git push origin master` to submit your solution
   to CodeCrafters. Test output will be streamed to your terminal.

# 1. Torrent File Information:

### Navigate to the `app` directory and run the following command. Make sure that your main.py and sample.torrent should be in the same directory.

```sh
python main.py info sample.torrent
```

# 2. Torrent File Information:

```sh
python main.py peers sample.torrent
```

# 3. Handshake with Peer:

```sh
python main.py handshake sample.torrent "your_any_one_peers_sample"  //for_example: 192.168.1.5:6881"
```

# 4. Download a Specific Piece:

```sh
python main.py download_piece -o piece1.dat sample.torrent 0
```

# 5. Download Entire Torrent:

```sh
python main.py download -o complete_file.dat sample.torrent

```
