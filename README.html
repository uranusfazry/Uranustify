<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pemutar Musik Hibrida</title>
    
    <!-- Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css">
    <!-- Font untuk Watermark -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@400;500;700&display=swap" rel="stylesheet">
    
    <!-- Scripts -->
    <script src="https://cdn.tailwindcss.com"></script>

    <style>
        /* --- Global Styles --- */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0d0f1c;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            padding: 20px;
            box-sizing: border-box;
            gap: 1.5rem;
            overflow-x: hidden;
        }

        /* --- Mode Switcher --- */
        .mode-switcher-container { display: flex; background-color: #2D2D42; border-radius: 1rem; padding: 0.25rem; width: 100%; max-width: 450px; }
        .mode-button { flex: 1; padding: 0.75rem 0.5rem; border: none; background-color: transparent; color: #A0AEC0; font-weight: 600; border-radius: 0.875rem; cursor: pointer; transition: all 0.3s ease; }
        .mode-button.active { background-color: #F43F8A; color: #FFFFFF; box-shadow: 0 4px 10px -2px rgba(244, 63, 138, 0.4); }

        /* --- STYLES FOR ONLINE PLAYER --- */
        #online-player-view .music-player-container { background-color: #1a1c2e; border-radius: 1.5rem; box-shadow: 0 25px 60px rgba(0, 0, 0, 0.4); padding: 2rem; width: 100%; max-width: 450px; color: #e0e6ed; display: flex; flex-direction: column; gap: 1.5rem; }
        #online-player-view .now-playing-section { background: linear-gradient(135deg, #4a148c, #6a1b9a); border-radius: 1rem; padding: 2.5rem 1.5rem; text-align: center; box-shadow: inset 0 2px 5px rgba(0,0,0,0.2), 0 5px 15px rgba(0,0,0,0.3); position: relative; overflow: hidden; }
        #online-player-view .now-playing-section::before { content: ''; position: absolute; top: -50%; left: -50%; width: 200%; height: 200%; background: radial-gradient(circle at center, rgba(255,255,255,0.05) 0%, transparent 70%); animation: rotateBg 20s linear infinite; }
        @keyframes rotateBg { from { transform: rotate(0deg); } to { transform: rotate(360deg); } }
        #online-player-view .now-playing-section h2 { font-size: 1.875rem; font-weight: 700; margin-bottom: 0.25rem; color: #ffffff; text-shadow: 0 1px 3px rgba(0,0,0,0.2); }
        #online-player-view .now-playing-section p { font-size: 1.125rem; color: #e0f2f7; font-weight: 400; }
        #online-player-view .audio-controls { background-color: #212338; border-radius: 1rem; padding: 1.5rem; display: flex; flex-direction: column; align-items: center; gap: 1.5rem; }
        #online-player-view .progress-bar-container { width: 100%; display: flex; align-items: center; gap: 0.75rem; color: #b0b8c0; font-size: 0.875rem; }
        #online-player-view .playback-buttons { display: flex; align-items: center; justify-content: center; width: 100%; gap: 1.5rem; }
        #online-player-view .control-button { background: none; border: none; color: #b0b8c0; font-size: 1.5rem; cursor: pointer; transition: color 0.2s ease, transform 0.2s ease; }
        #online-player-view .control-button:hover { color: #ffffff; transform: scale(1.05); }
        #online-player-view .control-button.active { color: #22c55e; }
        #online-player-view .play-pause-button { background-color: #22c55e; color: #ffffff; width: 60px; height: 60px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 2rem; box-shadow: 0 5px 15px rgba(34, 197, 94, 0.4); transition: all 0.2s ease; }
        #online-player-view .play-pause-button:hover { background-color: #16a34a; transform: scale(1.05); }
        #online-player-view .playlist-section { background-color: #212338; border-radius: 1rem; padding: 1.5rem; display: flex; flex-direction: column; gap: 1rem; }
        #playlistHeader { display: flex; justify-content: space-between; align-items: center; cursor: pointer; }
        #playlistHeader h3 { font-size: 1.25rem; font-weight: 600; color: #ffffff; }
        #playlistToggleIcon { transition: transform 0.3s ease; }
        #playlistToggleIcon.rotate-180 { transform: rotate(180deg); }
        #onlinePlaylist { transition: max-height 0.3s ease-out, opacity 0.3s ease-out; overflow: hidden; }
        #onlinePlaylist.hidden { max-height: 0 !important; opacity: 0; }
        #online-player-view .playlist-item { background-color: #2c2e42; border-radius: 0.75rem; padding: 1rem 1.25rem; display: flex; justify-content: space-between; align-items: center; cursor: pointer; transition: all 0.2s ease; }
        #online-player-view .playlist-item:hover { background-color: #3e415a; transform: translateY(-2px); }
        #online-player-view .playlist-item.active { background-color: #3a3c5a; border: 1px solid #6366f1; }
        #online-player-view .playlist-item.playing h4 { color: #22c55e; }
        #online-player-view .playlist-item-info { flex-grow: 1; }
        #online-player-view .playlist-item-info h4 { font-size: 1rem; font-weight: 600; color: #ffffff; transition: color 0.2s ease; }
        #online-player-view .playlist-item-info p { font-size: 0.875rem; color: #a0aec0; }
        #online-player-view .playlist-item-actions a { color: #b0b8c0; font-size: 1.1rem; transition: color 0.2s ease; }
        #online-player-view .playlist-item-actions a:hover { color: #ffffff; }

        /* --- STYLES FOR OFFLINE PLAYER --- */
        #offline-player-view .music-player-container { background-color: #1C1C2D; border-radius: 1.5rem; box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.5); width: 100%; max-width: 400px; color: #FFFFFF; display: flex; flex-direction: column; overflow: hidden; }
        #offline-player-view #visualizer { width: 100%; height: 180px; display: block; background-color: #1C1C2D; }
        #offline-player-view .song-info { padding: 1.5rem 2rem; text-align: center; }
        #offline-player-view .song-info h2 { font-size: 1.75rem; font-weight: 700; margin-bottom: 0.25rem; white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }
        #offline-player-view .song-info p { font-size: 1rem; color: #A0AEC0; }
        #offline-player-view .controls-section { padding: 1.5rem 2rem; display: flex; flex-direction: column; gap: 1.5rem; }
        #offline-player-view .playback-buttons { display: flex; align-items: center; justify-content: center; gap: 1rem; width: 100%; }
        #offline-player-view .control-button { background: none; border: none; color: #A0AEC0; font-size: 1.25rem; cursor: pointer; transition: color 0.2s ease, transform 0.2s ease; }
        #offline-player-view .control-button:hover { color: #FFFFFF; }
        #offline-player-view .control-button.active { color: #F43F8A; }
        #offline-player-view .play-pause-button { background-color: #F43F8A; color: #ffffff; width: 60px; height: 60px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 2rem; box-shadow: 0 10px 20px -5px rgba(244, 63, 138, 0.4); transition: all 0.2s ease; margin: 0 1rem; }
        #offline-player-view .play-pause-button:hover { transform: scale(1.05); }
        #offline-player-view .playlist-upload-section { padding: 1.5rem 2rem; display: flex; flex-direction: column; gap: 1rem; }
        #offlineSongList { max-height: 110px; overflow-y: auto; display: flex; flex-direction: column; gap: 0.75rem; padding-right: 8px; margin-right: -8px; }
        #offlineSongList::-webkit-scrollbar { width: 6px; }
        #offlineSongList::-webkit-scrollbar-track { background: #2D2D42; border-radius: 3px; }
        #offlineSongList::-webkit-scrollbar-thumb { background: #5c5c7a; border-radius: 3px; }
        #offlineSongList::-webkit-scrollbar-thumb:hover { background: #7a7a9c; }
        #offline-player-view .action-button { width: 100%; padding: 0.875rem 1rem; border-radius: 0.75rem; border: none; font-size: 1rem; font-weight: 600; cursor: pointer; transition: all 0.2s ease; flex-shrink: 0; }
        #offline-player-view #uploadButton { background-color: #2D2D42; color: #FFFFFF; }
        #offline-player-view .playlist-item-button { background-color: #2D2D42; color: #FFFFFF; white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }
        #offline-player-view .playlist-item-button.active { background-color: #F43F8A; }

        /* --- SHARED STYLES FOR VOLUME & PROGRESS --- */
        .volume-control-container { width: 100%; display: flex; align-items: center; gap: 0.75rem; color: #b0b8c0; }
        .volume-icon-btn { background: none; border: none; color: #b0b8c0; font-size: 1.25rem; cursor: pointer; padding: 0.25rem; }
        .volume-slider-wrapper { display: flex; flex-grow: 1; align-items: center; gap: 0.75rem; transition: max-height 0.3s ease, opacity 0.3s ease; max-height: 50px; opacity: 1; overflow: hidden; }
        .volume-slider-wrapper.hidden { max-height: 0; opacity: 0; }
        .volume-control { -webkit-appearance: none; flex-grow: 1; height: 5px; background: #3e415a; border-radius: 2.5px; outline: none; cursor: pointer; }
        .volume-control::-webkit-slider-thumb { -webkit-appearance: none; width: 16px; height: 16px; background: #a0aec0; border-radius: 50%; cursor: pointer; transition: background 0.2s; }
        .volume-control::-webkit-slider-thumb:hover { background: #ffffff; }
        .volume-percentage { font-size: 0.875rem; width: 45px; text-align: right; }
        
        .progress-bar { -webkit-appearance: none; width: 100%; height: 6px; border-radius: 3px; outline: none; cursor: pointer; transition: background 0.1s linear; }
        .progress-bar::-webkit-slider-thumb { -webkit-appearance: none; width: 16px; height: 16px; border-radius: 50%; cursor: pointer; border: 0; }
        #onlineAudioProgress::-webkit-slider-thumb { background: #22c55e; }
        #offlineAudioProgress::-webkit-slider-thumb { background: #F43F8A; }

        /* --- STYLES FOR FUTURISTIC WATERMARK --- */
        :root {
            --glow-color: hsl(186, 100%, 50%);
            --background-color: rgba(10, 25, 40, 0.85);
            --border-color: rgba(127, 255, 212, 0.3);
            --text-color: rgba(230, 255, 255, 0.95);
            --particle-base-hue: 186;
            --particle-base-lightness: 60;
        }

        @keyframes slideUpFadeIn {
            from { opacity: 0; transform: translateY(15px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes logo3DFlip {
            0% { transform: rotateY(0deg); filter: brightness(1); }
            50% { transform: rotateY(180deg); filter: brightness(2) drop-shadow(0 0 8px var(--glow-color)); }
            100% { transform: rotateY(360deg); filter: brightness(1); }
        }
        
        #futuristic-watermark {
            position: fixed;
            bottom: 25px;
            left: 25px;
            padding: 8px 15px;
            min-width: 212px;
            background: var(--background-color);
            color: var(--text-color);
            font-family: 'Roboto Mono', monospace;
            font-weight: 500;
            backdrop-filter: blur(18px);
            -webkit-backdrop-filter: blur(18px);
            border: 1px solid var(--border-color);
            border-radius: 10px;
            box-shadow: 0 0 15px rgba(var(--glow-color), 0.15), 0 0 30px rgba(var(--glow-color), 0.1), inset 0 0 10px rgba(var(--glow-color), 0.1);
            z-index: 9999;
            cursor: pointer;
            user-select: none;
            overflow: hidden;
            opacity: 0;
            animation: slideUpFadeIn 1s ease-out 0.5s forwards;
            transition: background-color 0.5s ease, color 0.5s ease, transform 0.3s ease, box-shadow 0.3s ease, border-color 0.3s ease;
        }
        
        #futuristic-watermark:hover {
            transform: translateY(-5px) scale(1.03);
            border-color: rgba(127, 255, 212, 0.8);
            box-shadow: 0 0 25px rgba(var(--glow-color), 0.4), 0 0 50px rgba(var(--glow-color), 0.25), inset 0 0 12px rgba(var(--glow-color), 0.2);
        }

        #futuristic-watermark.light-mode {
            --glow-color: hsl(220, 90%, 60%);
            --background-color: rgba(245, 248, 252, 0.85);
            --border-color: rgba(60, 100, 150, 0.3);
            --text-color: rgba(10, 25, 40, 0.95);
            --particle-base-hue: 220;
            --particle-base-lightness: 40;
        }
        
        #particle-canvas {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 1;
            pointer-events: none;
        }

        .f-content-wrapper {
            position: relative;
            z-index: 2;
            display: flex;
            align-items: center;
            justify-content: center;
            min-height: 18px;
        }

        .f-content {
            display: flex;
            align-items: center;
            gap: 10px;
            transition: opacity 0.4s ease, transform 0.4s ease;
        }

        .f-content.hidden {
            opacity: 0;
            pointer-events: none;
            position: absolute;
            transform: scale(0.9);
        }

        .f-logo-container {
            width: 18px;
            height: 18px;
            transition: transform 0.4s ease;
            flex-shrink: 0;
        }

        .f-logo-container.reacting {
            animation: logo3DFlip 0.7s cubic-bezier(0.22, 1, 0.36, 1);
        }
        
        .f-logo-container svg {
            width: 100%;
            height: 100%;
            stroke: var(--glow-color);
            stroke-width: 8;
            transition: stroke 0.5s ease;
        }
        
        #f-watermark-text, #f-follow-message {
            transition: color 0.5s ease;
        }

        #f-watermark-text {
            font-size: 12px;
            letter-spacing: 1px;
            text-transform: uppercase;
        }
        
        #f-follow-message {
            font-size: 11px;
            letter-spacing: 0.2px;
            font-weight: 700;
            text-align: center;
            white-space: nowrap;
        }
    </style>
</head>
<body>

    <div class="mode-switcher-container">
        <button class="mode-button active" id="onlineModeBtn">Online</button>
        <button class="mode-button" id="offlineModeBtn">Offline</button>
    </div>

    <div id="online-player-view">
        <div class="music-player-container">
            <div class="now-playing-section">
                <h2 id="onlineSongTitle">Pilih Lagu</h2>
                <p id="onlineSongArtist">...</p>
            </div>
            <div class="audio-controls">
                <div class="progress-bar-container">
                    <span id="onlineCurrentTime">0:00</span>
                    <input type="range" id="onlineAudioProgress" class="progress-bar" value="0" min="0" max="0" step="0.01">
                    <span id="onlineDuration">0:00</span>
                </div>
                <div class="playback-buttons">
                    <button class="control-button" id="onlineShuffleButton" title="Putar Acak"><i class="fas fa-random"></i></button>
                    <button class="control-button" id="onlinePrevButton"><i class="fas fa-backward"></i></button>
                    <button class="play-pause-button" id="onlinePlayPauseButton"><i class="fas fa-play"></i></button>
                    <button class="control-button" id="onlineNextButton"><i class="fas fa-forward"></i></button>
                    <button class="control-button" id="onlineRepeatButton" title="Ulangi"><i class="fas fa-redo"></i></button>
                </div>
                <div class="volume-control-container">
                    <button id="onlineVolumeIconBtn" class="volume-icon-btn"><i class="fas fa-volume-high"></i></button>
                    <div id="onlineVolumeSliderWrapper" class="volume-slider-wrapper hidden">
                        <input type="range" id="onlineVolumeControl" class="volume-control" min="0" max="1" step="0.01" value="1">
                        <span id="onlineVolumePercentage" class="volume-percentage">100%</span>
                    </div>
                </div>
            </div>
            <div class="playlist-section">
                <div id="playlistHeader">
                    <h3>Daftar Putar</h3>
                    <i id="playlistToggleIcon" class="fas fa-chevron-down"></i>
                </div>
                <div id="onlinePlaylist" class="hidden"></div>
            </div>
        </div>
        <audio id="audioPlayerOnline" preload="auto"></audio>
    </div>

    <div id="offline-player-view" style="display: none;">
        <div class="music-player-container">
            <canvas id="visualizer"></canvas>
            <div class="song-info">
                <h2 id="offlineSongTitle">Pilih Lagu</h2>
                <p id="offlineSongArtist">untuk memulai</p>
            </div>
            <div class="controls-section">
                <div class="progress-bar-container">
                    <span id="offlineCurrentTime">0:00</span>
                    <input type="range" id="offlineAudioProgress" class="progress-bar" value="0" min="0" max="0" step="0.01">
                    <span id="offlineDuration">0:00</span>
                </div>
                <div class="playback-buttons">
                    <button class="control-button" id="offlineShuffleButton" title="Putar Acak"><i class="fas fa-random"></i></button>
                    <button class="control-button" id="offlinePrevButton"><i class="fas fa-backward-step"></i></button>
                    <button class="play-pause-button" id="offlinePlayPauseButton"><i class="fas fa-play"></i></button>
                    <button class="control-button" id="offlineNextButton"><i class="fas fa-forward-step"></i></button>
                    <button class="control-button" id="offlineRepeatButton" title="Ulangi"><i class="fas fa-redo"></i></button>
                </div>
                 <div class="volume-control-container">
                    <button id="offlineVolumeIconBtn" class="volume-icon-btn"><i class="fas fa-volume-high"></i></button>
                    <div id="offlineVolumeSliderWrapper" class="volume-slider-wrapper hidden">
                        <input type="range" id="offlineVolumeControl" class="volume-control" min="0" max="1" step="0.01" value="1">
                        <span id="offlineVolumePercentage" class="volume-percentage">100%</span>
                    </div>
                </div>
            </div>
            <div class="playlist-upload-section">
                 <button id="uploadButton" class="action-button"><i class="fas fa-upload mr-2"></i> Unggah Musik</button>
                 <div id="offlineSongList"></div>
            </div>
        </div>
        <input type="file" id="uploadInput" multiple accept="audio/*" class="hidden">
        <audio id="audioPlayerOffline" preload="auto" crossOrigin="anonymous"></audio>
    </div>

    <script>
        // --- MUSIC PLAYER SCRIPT ---
        // Global control
        const onlineModeBtn = document.getElementById('onlineModeBtn');
        const offlineModeBtn = document.getElementById('offlineModeBtn');
        const onlineView = document.getElementById('online-player-view');
        const offlineView = document.getElementById('offline-player-view');

        function switchMode(mode) {
            if (mode === 'online') {
                onlineView.style.display = 'block';
                offlineView.style.display = 'none';
                onlineModeBtn.classList.add('active');
                offlineModeBtn.classList.remove('active');
                offlinePlayer.pause();
                onlinePlayer.init(); 
            } else { // offline
                onlineView.style.display = 'none';
                offlineView.style.display = 'block';
                onlineModeBtn.classList.remove('active');
                offlineModeBtn.classList.add('active');
                onlinePlayer.pause();
                offlinePlayer.init(); 
            }
        }

        // Online player module
        const onlinePlayer = {
            isInitialized: false,
            currentSongIndex: 0,
            isShuffle: false,
            isRepeat: false,
            songs: [
                { title: 'Chammak Challo', artist: 'uranusfazry', src: 'https://c.top4top.io/m_3457ukcau0.mp3' },
                { title: 'DJ CAMPURAN VIRAL', artist: 'uranusfazry', src: 'https://h.top4top.io/m_345748hje1.mp3' },
                { title: 'Chammak Satu', artist: 'uranusfazry', src: 'https://h.top4top.io/m_3467gl85x1.m4a' },
                { title: 'DJ CAMPURAN VIRAL 2', artist: 'uranusfazry', src: 'https://k.top4top.io/m_3458s4twa1.m4a' }
            ],

            init() {
                if (this.isInitialized) return;
                this.audioPlayer = document.getElementById('audioPlayerOnline');
                this.playPauseButton = document.getElementById('onlinePlayPauseButton');
                this.prevButton = document.getElementById('onlinePrevButton');
                this.nextButton = document.getElementById('onlineNextButton');
                this.shuffleButton = document.getElementById('onlineShuffleButton');
                this.repeatButton = document.getElementById('onlineRepeatButton');
                this.volumeIconBtn = document.getElementById('onlineVolumeIconBtn');
                this.volumeSliderWrapper = document.getElementById('onlineVolumeSliderWrapper');
                this.volumeControl = document.getElementById('onlineVolumeControl');
                this.volumePercentage = document.getElementById('onlineVolumePercentage');
                this.audioProgress = document.getElementById('onlineAudioProgress');
                this.currentTimeSpan = document.getElementById('onlineCurrentTime');
                this.durationSpan = document.getElementById('onlineDuration');
                this.currentSongTitle = document.getElementById('onlineSongTitle');
                this.currentSongArtist = document.getElementById('onlineSongArtist');
                this.playlistHeader = document.getElementById('playlistHeader');
                this.playlistToggleIcon = document.getElementById('playlistToggleIcon');
                this.playlistDiv = document.getElementById('onlinePlaylist');
                this.addEventListeners();
                this.populatePlaylist();
                if (this.songs.length > 0) this.loadSong(this.currentSongIndex);
                this.isInitialized = true;
            },

            addEventListeners() {
                this.playPauseButton.addEventListener('click', () => this.togglePlayPause());
                this.nextButton.addEventListener('click', () => this.playNextSong());
                this.prevButton.addEventListener('click', () => this.playPrevSong());
                this.shuffleButton.addEventListener('click', (e) => this.toggleShuffle(e.currentTarget));
                this.repeatButton.addEventListener('click', (e) => this.toggleRepeat(e.currentTarget));
                this.volumeIconBtn.addEventListener('click', () => this.toggleVolumeSlider());
                this.volumeControl.addEventListener('input', (e) => this.setVolume(e.target.value));
                this.playlistHeader.addEventListener('click', () => this.togglePlaylist());
                this.audioPlayer.addEventListener('timeupdate', () => this.updateProgress());
                this.audioPlayer.addEventListener('loadedmetadata', () => this.updateDuration());
                this.audioPlayer.addEventListener('ended', () => this.handleSongEnd());
                this.audioProgress.addEventListener('input', (e) => this.seek(e));
                this.audioPlayer.addEventListener('play', () => this.updatePlayState());
                this.audioPlayer.addEventListener('pause', () => this.updatePlayState());
            },

            loadSong(index) {
                const song = this.songs[index];
                this.audioPlayer.src = song.src;
                this.currentSongTitle.textContent = song.title;
                this.currentSongArtist.textContent = song.artist;
                this.audioPlayer.load();
                this.updatePlaylistActiveState(index);
                this.updateProgress();
            },

            async togglePlayPause() { if (this.audioPlayer.paused) { await this.audioPlayer.play(); } else { this.audioPlayer.pause(); } },
            pause() { if(this.audioPlayer) this.audioPlayer.pause(); },

            playNextSong() {
                if(this.songs.length === 0) return;
                if (this.isShuffle) { let newIndex; do { newIndex = Math.floor(Math.random() * this.songs.length); } while (this.songs.length > 1 && newIndex === this.currentSongIndex); this.currentSongIndex = newIndex; } else { this.currentSongIndex = (this.currentSongIndex + 1) % this.songs.length; }
                this.loadSong(this.currentSongIndex);
                this.audioPlayer.play();
            },

            playPrevSong() {
                if(this.songs.length === 0) return;
                this.currentSongIndex = (this.currentSongIndex - 1 + this.songs.length) % this.songs.length;
                this.loadSong(this.currentSongIndex);
                this.audioPlayer.play();
            },

            handleSongEnd() { if (this.isRepeat) { this.audioPlayer.currentTime = 0; this.audioPlayer.play(); } else { this.playNextSong(); } },
            toggleShuffle(button) { this.isShuffle = !this.isShuffle; button.classList.toggle('active', this.isShuffle); },
            toggleRepeat(button) { this.isRepeat = !this.isRepeat; button.classList.toggle('active', this.isRepeat); },
            toggleVolumeSlider() { this.volumeSliderWrapper.classList.toggle('hidden'); },
            togglePlaylist() { this.playlistDiv.classList.toggle('hidden'); this.playlistToggleIcon.classList.toggle('rotate-180'); },
            setVolume(value) { this.audioPlayer.volume = value; this.volumePercentage.textContent = `${Math.round(value * 100)}%`; },
            
            populatePlaylist() {
                this.playlistDiv.innerHTML = '';
                this.songs.forEach((song, index) => {
                    const item = document.createElement('div');
                    item.className = 'playlist-item';
                    item.setAttribute('data-index', index);
                    item.innerHTML = `<div class="playlist-item-info"><h4>${song.title}</h4><p>${song.artist}</p></div><div class="playlist-item-actions"><a href="${song.src}" target="_blank" rel="noopener noreferrer" download="${song.artist} - ${song.title}.mp3" class="download-link" title="Unduh" onclick="event.stopPropagation()"><i class="fas fa-download"></i></a></div>`;
                    item.addEventListener('click', () => { this.currentSongIndex = index; this.loadSong(this.currentSongIndex); this.audioPlayer.play(); });
                    this.playlistDiv.appendChild(item);
                });
                this.updatePlaylistActiveState(this.currentSongIndex);
            },

            updatePlaylistActiveState(activeIndex) {
                document.querySelectorAll('#online-player-view .playlist-item').forEach((item, index) => {
                    item.classList.remove('active', 'playing');
                    if (index === activeIndex) { item.classList.add('active'); if (!this.audioPlayer.paused) { item.classList.add('playing'); } }
                });
            },
            
            updatePlayState() { this.playPauseButton.innerHTML = this.audioPlayer.paused ? '<i class="fas fa-play"></i>' : '<i class="fas fa-pause"></i>'; this.updatePlaylistActiveState(this.currentSongIndex); },
            formatTime: (s) => isNaN(s) ? '0:00' : `${Math.floor(s/60)}:${Math.floor(s%60).toString().padStart(2,'0')}`,
            updateProgress() { 
                const progressPercent = (this.audioPlayer.currentTime / this.audioPlayer.duration) * 100 || 0;
                this.audioProgress.style.background = `linear-gradient(to right, #22c55e ${progressPercent}%, #3e415a ${progressPercent}%)`;
                this.audioProgress.value = this.audioPlayer.currentTime; 
                this.currentTimeSpan.textContent = this.formatTime(this.audioPlayer.currentTime); 
            },
            updateDuration() { if (!isNaN(this.audioPlayer.duration)) { this.durationSpan.textContent = this.formatTime(this.audioPlayer.duration); this.audioProgress.max = this.audioPlayer.duration; } },
            seek(e) { this.audioPlayer.currentTime = e.target.value; this.updateProgress(); },
        };

        // Offline player module
        const offlinePlayer = {
            isInitialized: false,
            currentSongIndex: 0,
            songs: [],
            isShuffle: false,
            isRepeat: false,
            audioContext: null, analyser: null, source: null, isAudioContextSetup: false,

            init() {
                if (this.isInitialized) return;
                this.audioPlayer = document.getElementById('audioPlayerOffline');
                this.playPauseButton = document.getElementById('offlinePlayPauseButton');
                this.prevButton = document.getElementById('offlinePrevButton');
                this.nextButton = document.getElementById('offlineNextButton');
                this.shuffleButton = document.getElementById('offlineShuffleButton');
                this.repeatButton = document.getElementById('offlineRepeatButton');
                this.volumeIconBtn = document.getElementById('offlineVolumeIconBtn');
                this.volumeSliderWrapper = document.getElementById('offlineVolumeSliderWrapper');
                this.volumeControl = document.getElementById('offlineVolumeControl');
                this.volumePercentage = document.getElementById('offlineVolumePercentage');
                this.audioProgress = document.getElementById('offlineAudioProgress');
                this.currentTimeSpan = document.getElementById('offlineCurrentTime');
                this.durationSpan = document.getElementById('offlineDuration');
                this.currentSongTitle = document.getElementById('offlineSongTitle');
                this.currentSongArtist = document.getElementById('offlineSongArtist');
                this.songListDiv = document.getElementById('offlineSongList');
                this.uploadButton = document.getElementById('uploadButton');
                this.uploadInput = document.getElementById('uploadInput');
                this.canvas = document.getElementById('visualizer');
                this.canvasCtx = this.canvas.getContext('2d');
                this.addEventListeners();
                this.handleResize();
                this.drawVisualizer();
                this.updateProgress();
                this.isInitialized = true;
            },
            
            pause() { if(this.audioPlayer) this.audioPlayer.pause(); },

            addEventListeners() {
                this.playPauseButton.addEventListener('click', () => this.togglePlayPause());
                this.nextButton.addEventListener('click', () => this.playNextSong());
                this.prevButton.addEventListener('click', () => this.playPrevSong());
                this.shuffleButton.addEventListener('click', (e) => this.toggleShuffle(e.currentTarget));
                this.repeatButton.addEventListener('click', (e) => this.toggleRepeat(e.currentTarget));
                this.volumeIconBtn.addEventListener('click', () => this.toggleVolumeSlider());
                this.volumeControl.addEventListener('input', (e) => this.setVolume(e.target.value));
                this.uploadButton.addEventListener('click', () => this.uploadInput.click());
                this.uploadInput.addEventListener('change', (e) => this.handleFileUpload(e));
                this.audioPlayer.addEventListener('timeupdate', () => this.updateProgress());
                this.audioPlayer.addEventListener('loadedmetadata', () => this.updateDuration());
                this.audioPlayer.addEventListener('ended', () => this.handleSongEnd());
                this.audioProgress.addEventListener('input', (e) => this.seek(e));
                this.audioPlayer.addEventListener('play', () => this.playPauseButton.innerHTML = '<i class="fas fa-pause"></i>');
                this.audioPlayer.addEventListener('pause', () => this.playPauseButton.innerHTML = '<i class="fas fa-play"></i>');
                window.addEventListener('resize', () => this.handleResize());
            },
            
            async togglePlayPause() {
                if (this.songs.length === 0) return;
                if (!this.isAudioContextSetup) this.setupAudioContext();
                if (this.audioContext && this.audioContext.state === 'suspended') await this.audioContext.resume();
                if (this.audioPlayer.paused) { await this.audioPlayer.play(); } else { this.audioPlayer.pause(); }
            },

            loadSong(index) {
                const song = this.songs[index];
                this.audioPlayer.src = song.src;
                this.currentSongTitle.textContent = song.title;
                this.currentSongArtist.textContent = song.artist;
                this.audioPlayer.load();
                this.populatePlaylist();
                this.updateProgress();
            },

            playNextSong() {
                if(this.songs.length === 0) return;
                if (this.isShuffle) { let newIndex; do { newIndex = Math.floor(Math.random() * this.songs.length); } while (this.songs.length > 1 && newIndex === this.currentSongIndex); this.currentSongIndex = newIndex; } else { this.currentSongIndex = (this.currentSongIndex + 1) % this.songs.length; }
                this.loadSong(this.currentSongIndex);
                this.audioPlayer.play();
            },
            
            playPrevSong() {
                if(this.songs.length === 0) return;
                this.currentSongIndex = (this.currentSongIndex - 1 + this.songs.length) % this.songs.length;
                this.loadSong(this.currentSongIndex);
                this.audioPlayer.play();
            },
            
            handleSongEnd() { if (this.isRepeat) { this.audioPlayer.currentTime = 0; this.audioPlayer.play(); } else { this.playNextSong(); } },
            toggleShuffle(button) { this.isShuffle = !this.isShuffle; button.classList.toggle('active', this.isShuffle); },
            toggleRepeat(button) { this.isRepeat = !this.isRepeat; button.classList.toggle('active', this.isRepeat); },
            toggleVolumeSlider() { this.volumeSliderWrapper.classList.toggle('hidden'); },
            setVolume(value) { this.audioPlayer.volume = value; this.volumePercentage.textContent = `${Math.round(value * 100)}%`; },
            
            handleFileUpload(event) {
                const files = event.target.files;
                if (!files.length) return;
                const wasEmpty = this.songs.length === 0;
                for (const file of files) { this.songs.push({ title: file.name.replace(/\.[^/.]+$/, ""), artist: 'File Lokal', src: URL.createObjectURL(file) }); }
                this.populatePlaylist();
                if (wasEmpty) { this.currentSongIndex = 0; this.loadSong(0); }
                event.target.value = '';
            },
            
            populatePlaylist() {
                this.songListDiv.innerHTML = '';
                this.songs.forEach((song, index) => {
                    const button = document.createElement('button');
                    button.className = 'action-button playlist-item-button';
                    button.textContent = song.title;
                    if (index === this.currentSongIndex) button.classList.add('active');
                    button.addEventListener('click', () => { this.currentSongIndex = index; this.loadSong(index); this.togglePlayPause(); });
                    this.songListDiv.appendChild(button);
                });
            },

            formatTime: (s) => isNaN(s) ? '0:00' : `${Math.floor(s/60)}:${Math.floor(s%60).toString().padStart(2,'0')}`,
            updateProgress() {
                if (!isNaN(this.audioPlayer.duration)) { 
                    const progressPercent = (this.audioPlayer.currentTime / this.audioPlayer.duration) * 100 || 0;
                    this.audioProgress.style.background = `linear-gradient(to right, #F43F8A ${progressPercent}%, #3e415a ${progressPercent}%)`;
                    this.audioProgress.value = this.audioPlayer.currentTime; 
                    this.currentTimeSpan.textContent = this.formatTime(this.audioPlayer.currentTime); 
                } else {
                     this.audioProgress.style.background = `linear-gradient(to right, #F43F8A 0%, #3e415a 0%)`;
                }
            },
            updateDuration() { if (!isNaN(this.audioPlayer.duration)) { this.durationSpan.textContent = this.formatTime(this.audioPlayer.duration); this.audioProgress.max = this.audioPlayer.duration; } },
            seek(e) { if(this.songs.length > 0) this.audioPlayer.currentTime = e.target.value; this.updateProgress(); },
            handleResize() { this.canvas.width = this.canvas.clientWidth; this.canvas.height = this.canvas.clientHeight; },

            setupAudioContext() {
                if (this.isAudioContextSetup) return;
                try {
                    this.audioContext = new (window.AudioContext || window.webkitAudioContext)();
                    this.analyser = this.audioContext.createAnalyser();
                    this.analyser.fftSize = 256;
                    this.source = this.audioContext.createMediaElementSource(this.audioPlayer);
                    this.source.connect(this.analyser);
                    this.analyser.connect(this.audioContext.destination);
                    this.isAudioContextSetup = true;
                } catch (e) { console.error("Could not set up AudioContext:", e); }
            },

            drawVisualizer() {
                requestAnimationFrame(() => this.drawVisualizer());
                if (!this.isAudioContextSetup || this.audioPlayer.paused) { if(this.canvasCtx) this.canvasCtx.clearRect(0, 0, this.canvas.width, this.canvas.height); return; }
                const bufferLength = this.analyser.frequencyBinCount;
                const dataArray = new Uint8Array(bufferLength);
                this.analyser.getByteFrequencyData(dataArray);
                this.canvasCtx.clearRect(0, 0, this.canvas.width, this.canvas.height);
                const barWidth = (this.canvas.width / bufferLength) * 1.5;
                let x = 0;
                const gradient = this.canvasCtx.createLinearGradient(0, 0, 0, this.canvas.height);
                gradient.addColorStop(0, '#F43F8A');
                gradient.addColorStop(0.5, '#D434A3');
                gradient.addColorStop(1, '#A827BF');
                this.canvasCtx.fillStyle = gradient;
                for (let i = 0; i < bufferLength; i++) {
                    const barHeight = dataArray[i] * (this.canvas.height / 255);
                    this.canvasCtx.fillRect(x, this.canvas.height - barHeight, barWidth, barHeight);
                    x += barWidth + 2;
                }
            },
        };

        // --- INITIALIZATION ---
        window.onload = () => {
            onlineModeBtn.addEventListener('click', () => switchMode('online'));
            offlineModeBtn.addEventListener('click', () => switchMode('offline'));
            switchMode('online');
        };
    </script>

    <!-- FUTURISTIC WATERMARK SCRIPT -->
    <script>
      (function() {
        function initializeWatermark() {
            const watermarkHTML = `
              <div id="futuristic-watermark" title="Design by ©URANUSFAZRY">
                <canvas id="particle-canvas"></canvas>
                <div class="f-content-wrapper">
                  <div id="f-main-content" class="f-content">
                    <div class="f-logo-container">
                      <svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path d="M20 20 L80 20 L80 80 L20 80 Z" stroke-opacity="0.5"/>
                          <path d="M50 5 L95 50 L50 95 L5 50 Z"/>
                      </svg>
                    </div>
                    <span id="f-watermark-text">©URANUSFAZRY</span>
                  </div>
                  <div id="f-follow-content" class="f-content hidden">
                      <span id="f-follow-message"></span>
                  </div>
                </div>
              </div>
            `;
            document.body.insertAdjacentHTML('beforeend', watermarkHTML);

            const watermarkEl = document.getElementById('futuristic-watermark');
            const textEl = document.getElementById('f-watermark-text');
            const logoEl = watermarkEl.querySelector('.f-logo-container');
            const mainContentEl = document.getElementById('f-main-content');
            const followContentEl = document.getElementById('f-follow-content');
            const followMessageEl = document.getElementById('f-follow-message');
            
            let isAnimating = false;
            let autoPlayInterval = null;
            let currentSequence = 0;
            const sequenceActions = ['scramble', 'logo', 'youtube', 'tiktok', 'reset'];

            const canvas = document.getElementById('particle-canvas');
            const ctx = canvas.getContext('2d');
            let particles = [];
            const resizeCanvas = () => { if (watermarkEl) { canvas.width = watermarkEl.offsetWidth; canvas.height = watermarkEl.offsetHeight; } };
            class Particle {
                constructor() { this.reset(); this.baseSpeedX = (Math.random() - 0.5) * 0.5; this.baseSpeedY = (Math.random() - 0.5) * 0.5; this.speedX = this.baseSpeedX; this.speedY = this.baseSpeedY; }
                update() {
                    this.x += this.speedX; this.y += this.speedY; this.opacity -= this.fadeSpeed;
                    if (this.opacity <= 0 || this.x < 0 || this.x > canvas.width || this.y < 0 || this.y > canvas.height) { this.reset(); }
                }
                draw() {
                    const style = getComputedStyle(watermarkEl);
                    const hue = style.getPropertyValue('--particle-base-hue').trim();
                    const lightness = parseFloat(style.getPropertyValue('--particle-base-lightness').trim());
                    ctx.globalAlpha = this.opacity;
                    ctx.fillStyle = `hsl(${hue}, 100%, ${lightness + this.opacity * 40}%)`;
                    ctx.beginPath(); ctx.arc(this.x, this.y, this.size, 0, Math.PI * 2); ctx.fill();
                }
                reset() { this.x = Math.random() * canvas.width; this.y = Math.random() * canvas.height; this.opacity = Math.random() * 0.5 + 0.2; this.size = Math.random() * 1.5 + 0.5; this.fadeSpeed = Math.random() * 0.015 + 0.005; }
            }
            const animateParticles = () => { ctx.clearRect(0, 0, canvas.width, canvas.height); particles.forEach(p => { p.update(); p.draw(); }); ctx.globalAlpha = 1.0; requestAnimationFrame(animateParticles); };
            
            const textScramble = (el) => {
                const originalText = "©URANUSFAZRY";
                const chars = '!<>*#{}[]'; let frame = 0; isAnimating = true;
                const interval = setInterval(() => {
                    el.innerText = originalText.split('').map((char, i) => { const p = (frame - i * 2) / 15; if (p < 0) return ' '; if (p > 1) return char; return chars[Math.floor(Math.random() * chars.length)]; }).join('');
                    if (frame >= originalText.length * 2 + 15) { clearInterval(interval); el.innerText = originalText; isAnimating = false; } frame++;
                }, 30);
            };

            const typewriter = (el, text) => {
                let i = 0; el.innerHTML = ""; isAnimating = true;
                const interval = setInterval(() => {
                    if (i < text.length) { el.innerHTML += text.charAt(i); i++; } 
                    else { clearInterval(interval); isAnimating = false; }
                }, 50);
            };

            const runAutoSequence = () => {
                if (isAnimating) return;
                const action = sequenceActions[currentSequence];
                switch (action) {
                    case 'scramble': textScramble(textEl); break;
                    case 'logo':
                        isAnimating = true;
                        logoEl.classList.add('reacting');
                        logoEl.addEventListener('animationend', () => { logoEl.classList.remove('reacting'); isAnimating = false; }, { once: true });
                        break;
                    case 'youtube':
                        isAnimating = true;
                        mainContentEl.classList.add('hidden');
                        setTimeout(() => {
                            followContentEl.classList.remove('hidden');
                            typewriter(followMessageEl, "Follow uranusfazry YouTube");
                        }, 400);
                        break;
                    case 'tiktok': 
                        typewriter(followMessageEl, "Follow uranusfazry TikTok"); 
                        break;
                    case 'reset':
                        isAnimating = true;
                        followContentEl.classList.add('hidden');
                        setTimeout(() => {
                            mainContentEl.classList.remove('hidden');
                            isAnimating = false;
                        }, 400);
                        break;
                }
                currentSequence = (currentSequence + 1) % sequenceActions.length;
            };

            const startAutoPlay = () => {
                if (autoPlayInterval) clearInterval(autoPlayInterval);
                runAutoSequence();
                autoPlayInterval = setInterval(runAutoSequence, 3500);
            };

            watermarkEl.addEventListener('click', () => { watermarkEl.classList.toggle('light-mode'); });
            
            const init = () => {
                resizeCanvas();
                for (let i = 0; i < 40; i++) particles.push(new Particle());
                animateParticles();
                window.addEventListener('resize', resizeCanvas);
                startAutoPlay();
            };
            init();
        }

        if (document.readyState === 'loading') {
            document.addEventListener('DOMContentLoaded', initializeWatermark);
        } else {
            initializeWatermark();
        }
      })();
    </script>
</body>
</html>
