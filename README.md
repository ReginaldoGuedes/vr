<!DOCTYPE html>
<html>
<head>
    <title>Realidade Aumentada com Vídeo</title>
    <script src="https://aframe.io/releases/1.2.0/aframe.min.js"></script>
    <script src="https://cdn.jsdelivr.net/gh/AR-js-org/AR.js/aframe/build/aframe-ar.js"></script>
</head>
<body style="margin: 0; overflow: hidden;">
    <a-scene embedded arjs="sourceType: webcam; debugUIEnabled: false;">
        <!-- Marcador Hiro -->
        <a-marker preset="hiro">
            <!-- Vídeo como textura em um plano 3D -->
            <a-entity 
                geometry="primitive: plane; width: 4; height: 3;"
                material="src: url(https://drive.google.com/uc?id=1Kf4Jruu0g2nKTvEJmcbpdI-SQGK68LvZ); shader: flat;"
                position="0 0 0" rotation="-90 0 0">
            </a-entity>
        </a-marker>

        <!-- Câmera -->
        <a-entity camera></a-entity>
    </a-scene>
</body>
</html>
