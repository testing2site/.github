
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>...</title>
    <link href="https://vjs.zencdn.net/8.0.4/video-js.css" rel="stylesheet">
    <script disable-devtool-auto src='https://cdn.jsdelivr.net/npm/disable-devtool'></script>


    <style>
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #000;
            overflow: hidden;
        }

        video {
            width: 100%;
            height: 100%;
            max-width: 100vw;
            max-height: 100vh;
            object-fit: contain;
        }
    </style>
</head>

<body>
    <!-- Video.js Player -->
    <video id="video-player" class="video-js vjs-fill vjs-big-play-centered vjs-theme-fantasy" controls playsinline
        muted></video>
    <!-- <div class="watermark" id="watermark"></div>-->
    <!-- Video.js Library -->
    <script src="https://vjs.zencdn.net/8.0.4/video.min.js"></script>

    <script>
        const token = 'MTIzNA';
    
    // Setup before initializing the player
    if (window.videojs && window.videojs.Vhs) {
    videojs.Vhs.xhr.beforeRequest = function(options) {
    const url = options.uri || options.url;
    if (url && url.endsWith('.ts')) {
    const separator = url.includes('?') ? '&' : '?';
    options.uri = url + separator + 'token=' + encodeURIComponent(token);
    }
    return options;
    };
    }
        const servers = [
    { server: "cr1.crossbladenaruto.site/hls", path: "/stream.m3u8" },
	{ server: "cr2.cofecifec.site/hls", path: "/stream.m3u8" },
	{ server: "cr3.crossbladenaruto.site/hls", path: "/stream.m3u8" },
	{ server: "cr5.cofecifec.site/hls", path: "/stream.m3u8" },
	{ server: "cr6.crossbladenaruto.site/hls", path: "/stream.m3u8" },
	{ server: "cr9.cofecifec.site/hls", path: "/stream.m3u8" }
];


const sources = servers.map(server => `https://${server.server}${server.path}?token=${token}`);

let currentSourceIndex = Math.floor(Math.random() * sources.length);
let retryAttempts = 0;
const maxRetries = 2;
const bufferTimeout = 4000;
let bufferTimeoutId;
let player;

function initializePlayer() {
    console.log("Initializing Video.js player...");

    player = videojs("video-player", {
        techOrder: ["html5"],
        autoplay: true,
        muted: true,
        controls: true,
        playsinline: true,
        responsive: true,
        fluid: true,
        html5: {
            vhs: {
                enableLowLatency: true,
                experimentalBufferBasedABR: true,
            },
        },
    });

    loadSource(sources[currentSourceIndex]);


    player.on("waiting", handleBuffering);
    player.on("stalled", handleBuffering);


    player.on("playing", () => {
        console.log("Playing started.");
        clearTimeout(bufferTimeoutId);
    });


    player.on("error", handleError);
}

function loadSource(source) {
    console.log(`Loading source: ${source}`);
    clearTimeout(bufferTimeoutId);

    player.src({ type: "application/x-mpegURL", src: source });
    player.play();


    bufferTimeoutId = setTimeout(() => {
        console.warn(`Buffering too long on source: ${source}, switching...`);
        switchToNextSource();
    }, bufferTimeout);
}

function handleBuffering() {
    console.warn("Buffering detected...");
    clearTimeout(bufferTimeoutId);


    bufferTimeoutId = setTimeout(() => {
        console.warn("Buffering timeout reached, switching source...");
        switchToNextSource();
    }, bufferTimeout);
}

function handleError() {
    console.warn(`Error detected on source: ${sources[currentSourceIndex]}`);
    if (retryAttempts < maxRetries) {
        retryAttempts++;
        console.log(`Retrying source: ${sources[currentSourceIndex]}
            (Attempt ${retryAttempts})`);
        loadSource(sources[currentSourceIndex]);
    } else {
        console.log("Max retries reached, switching source...");
        switchToNextSource();
    }
}
function switchToNextSource() {
    retryAttempts = 0;
    currentSourceIndex = (currentSourceIndex + 1) % sources.length;
    console.log(`Switching to next source: ${sources[currentSourceIndex]}`);
    loadSource(sources[currentSourceIndex]);
}
document.addEventListener("DOMContentLoaded", initializePlayer);
    </script>
<script>
        
        document.addEventListener('contextmenu', e => e.preventDefault());
        
        
        document.addEventListener('keydown', e => {
        // F12
        if (e.key === 'F12') {
        e.preventDefault();
        }
        
        if (
        e.ctrlKey &&
        (e.shiftKey && ['I', 'J', 'C'].includes(e.key.toUpperCase())) ||
        e.key.toUpperCase() === 'U'
        ) {
        e.preventDefault();
        }
        });
        
        
        document.addEventListener('keydown', e => {
        if (e.ctrlKey && e.shiftKey && e.key.toUpperCase() === 'S') {
        e.preventDefault();
        }
        });
        
        
        setInterval(() => {
        let start = performance.now();
        debugger;
        let end = performance.now();
        if (end - start > 100) {
        
        alert('Devtools detected!');
        
        }
        }, 1000);
    </script>

</body>

</html>
