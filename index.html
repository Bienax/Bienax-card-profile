<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carte de Profil</title>
    <style>
        :root {
          --pointer-x: 50%;
          --pointer-y: 50%;
          --pointer-from-center: 0;
          --pointer-from-top: 0.5;
          --pointer-from-left: 0.5;
          --card-opacity: 0;
          --rotate-x: 0deg;
          --rotate-y: 0deg;
          --background-x: 50%;
          --background-y: 50%;
          --grain: none;
          --icon: none;
          --behind-gradient: none;
          --inner-gradient: none;
          --avatar-image: none;
          --sunpillar-1: hsl(2, 100%, 73%);
          --sunpillar-2: hsl(53, 100%, 69%);
          --sunpillar-3: hsl(93, 100%, 69%);
          --sunpillar-4: hsl(176, 100%, 76%);
          --sunpillar-5: hsl(228, 100%, 74%);
          --sunpillar-6: hsl(283, 100%, 73%);
          --sunpillar-clr-1: var(--sunpillar-1);
          --sunpillar-clr-2: var(--sunpillar-2);
          --sunpillar-clr-3: var(--sunpillar-3);
          --sunpillar-clr-4: var(--sunpillar-4);
          --sunpillar-clr-5: var(--sunpillar-5);
          --sunpillar-clr-6: var(--sunpillar-6);
          --card-radius: 30px;
        }

        * {
          margin: 0;
          padding: 0;
          box-sizing: border-box;
        }

        body {
          min-height: 100vh;
          background: linear-gradient(135deg, #0f172a 0%, #581c87 50%, #0f172a 100%);
          display: flex;
          align-items: center;
          justify-content: center;
          padding: 24px;
          font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
        }

        .container {
          position: relative;
        }

        .file-input {
          display: none;
        }

        .upload-zone {
          position: absolute;
          inset: 0;
          z-index: 50;
          display: flex;
          align-items: center;
          justify-content: center;
          cursor: pointer;
        }

        .upload-content {
          background: rgba(0, 0, 0, 0.8);
          backdrop-filter: blur(4px);
          border-radius: 9999px;
          padding: 32px;
          border: 2px dashed #22d3ee;
          text-align: center;
          transition: all 0.3s ease;
        }

        .upload-content:hover {
          border-color: #67e8f9;
        }

        .upload-icon {
          font-size: 60px;
          color: #22d3ee;
          margin-bottom: 16px;
          transition: transform 0.3s ease;
        }

        .upload-content:hover .upload-icon {
          transform: scale(1.1);
        }

        .upload-text {
          color: #22d3ee;
          font-weight: bold;
          font-size: 18px;
        }

        .upload-subtext {
          color: #67e8f9;
          font-size: 14px;
          margin-top: 8px;
        }

        .processing-overlay {
          position: absolute;
          inset: 0;
          z-index: 60;
          display: flex;
          align-items: center;
          justify-content: center;
          background: rgba(0, 0, 0, 0.5);
          backdrop-filter: blur(4px);
          border-radius: 24px;
        }

        .processing-content {
          background: rgba(0, 0, 0, 0.8);
          border-radius: 16px;
          padding: 24px;
          text-align: center;
        }

        .spinner {
          width: 48px;
          height: 48px;
          border: 2px solid transparent;
          border-bottom: 2px solid #22d3ee;
          border-radius: 50%;
          animation: spin 1s linear infinite;
          margin: 0 auto 16px;
        }

        @keyframes spin {
          to { transform: rotate(360deg); }
        }

        .processing-text {
          color: #22d3ee;
          font-weight: bold;
          margin-bottom: 8px;
        }

        .processing-subtext {
          color: #67e8f9;
          font-size: 14px;
        }

        .pc-card-wrapper {
          perspective: 500px;
          transform: translate3d(0, 0, 0.1px);
          position: relative;
          touch-action: none;
          --behind-gradient: radial-gradient(farthest-side circle at var(--pointer-x) var(--pointer-y),hsla(266,100%,90%,var(--card-opacity)) 4%,hsla(266,50%,80%,calc(var(--card-opacity)*0.75)) 10%,hsla(266,25%,70%,calc(var(--card-opacity)*0.5)) 50%,hsla(266,0%,60%,0) 100%),radial-gradient(35% 52% at 55% 20%,#00ffaac4 0%,#073aff00 100%),radial-gradient(100% 100% at 50% 50%,#00c1ffff 1%,#073aff00 76%),conic-gradient(from 124deg at 50% 50%,#c137ffff 0%,#07c6ffff 40%,#07c6ffff 60%,#c137ffff 100%);
          --inner-gradient: linear-gradient(145deg,#60496e8c 0%,#71C4FF44 100%);
        }

        .pc-card-wrapper::before {
          content: '';
          position: absolute;
          inset: -10px;
          background: inherit;
          background-position: inherit;
          border-radius: inherit;
          transition: all 0.5s ease;
          filter: contrast(2) saturate(2) blur(36px);
          transform: scale(0.8) translate3d(0, 0, 0.1px);
          background-size: 100% 100%;
          background-image: var(--behind-gradient);
        }

        .pc-card-wrapper:hover,
        .pc-card-wrapper.active {
          --card-opacity: 1;
        }

        .pc-card-wrapper:hover::before,
        .pc-card-wrapper.active::before {
          filter: contrast(1) saturate(2) blur(40px) opacity(1);
          transform: scale(0.9) translate3d(0, 0, 0.1px);
        }

        .pc-card {
          height: 80vh;
          max-height: 540px;
          display: grid;
          aspect-ratio: 0.718;
          border-radius: var(--card-radius);
          position: relative;
          background-blend-mode: color-dodge, normal, normal, normal;
          animation: glow-bg 12s linear infinite;
          box-shadow: rgba(0, 0, 0, 0.8) calc((var(--pointer-from-left) * 10px) - 3px) calc((var(--pointer-from-top) * 20px) - 6px) 20px -5px;
          transition: transform 1s ease;
          transform: translate3d(0, 0, 0.1px) rotateX(0deg) rotateY(0deg);
          background-size: 100% 100%;
          background-position: 0 0, 0 0, 50% 50%, 0 0;
          background-image: var(--behind-gradient);
          overflow: hidden;
        }

        .pc-card:hover,
        .pc-card.active {
          transition: none;
          transform: translate3d(0, 0, 0.1px) rotateX(var(--rotate-y)) rotateY(var(--rotate-x));
        }

        .pc-card > * {
          display: grid;
          grid-area: 1/-1;
          border-radius: var(--card-radius);
          transform: translate3d(0, 0, 0.1px);
          pointer-events: none;
        }

        .pc-inside {
          inset: 1px;
          position: absolute;
          background-image: var(--inner-gradient);
          background-color: rgba(0, 0, 0, 0.9);
          transform: translate3d(0, 0, 0.01px);
        }

        .pc-shine {
          mask-image: none;
          mask-mode: luminance;
          mask-repeat: repeat;
          mask-size: 150%;
          mask-position: top calc(200% - (var(--background-y) * 5)) left calc(100% - var(--background-x));
          transition: filter 0.6s ease;
          filter: brightness(0.66) contrast(1.33) saturate(0.33) opacity(0.4);
          animation: holo-bg 18s linear infinite;
          mix-blend-mode: color-dodge;
          --space: 5%;
          --angle: -45deg;
          transform: translate3d(0, 0, 1px);
          overflow: hidden;
          z-index: 3;
          background: transparent;
          background-size: cover;
          background-position: center;
          background-image: repeating-linear-gradient(0deg, var(--sunpillar-clr-1) calc(var(--space) * 1), var(--sunpillar-clr-2) calc(var(--space) * 2), var(--sunpillar-clr-3) calc(var(--space) * 3), var(--sunpillar-clr-4) calc(var(--space) * 4), var(--sunpillar-clr-5) calc(var(--space) * 5), var(--sunpillar-clr-6) calc(var(--space) * 6), var(--sunpillar-clr-1) calc(var(--space) * 7)), repeating-linear-gradient(var(--angle), #0e152e 0%, hsl(180, 10%, 60%) 3.8%, hsl(180, 29%, 66%) 4.5%, hsl(180, 10%, 60%) 5.2%, #0e152e 10%, #0e152e 12%), radial-gradient(farthest-corner circle at var(--pointer-x) var(--pointer-y), hsla(0, 0%, 0%, 0.1) 12%, hsla(0, 0%, 0%, 0.15) 20%, hsla(0, 0%, 0%, 0.25) 120%);
          background-position: 0 var(--background-y), var(--background-x) var(--background-y), center;
          background-blend-mode: color, hard-light;
          background-size: 500% 500%, 300% 300%, 200% 200%;
          background-repeat: repeat;
        }

        .pc-card:hover .pc-shine,
        .pc-card.active .pc-shine {
          filter: brightness(0.85) contrast(1.5) saturate(0.5) opacity(0.6);
        }

        .pc-glare {
          transform: translate3d(0, 0, 1.1px);
          overflow: hidden;
          background-image: radial-gradient(farthest-corner circle at var(--pointer-x) var(--pointer-y), hsl(248, 25%, 80%) 12%, hsla(207, 40%, 30%, 0.8) 90%);
          mix-blend-mode: overlay;
          filter: brightness(0.8) contrast(1.2);
          z-index: 4;
        }

        .pc-avatar-content {
          mix-blend-mode: normal;
          overflow: hidden;
          position: relative;
        }

        .avatar {
          width: 100%;
          position: absolute;
          left: 50%;
          transform: translateX(-50%) scale(1) !important;
          bottom: 0;
          top: 0;
          opacity: 1 !important;
          object-fit: contain;
          object-position: center;
          height: 100%;
          border-radius: var(--card-radius);
          z-index: 1;
          pointer-events: none;
          filter: none !important;
          transition: none !important;
        }

        .pc-avatar-content::before {
          content: "";
          position: absolute;
          inset: 0;
          z-index: 2;
          backdrop-filter: none;
          mask: linear-gradient(to bottom,
              rgba(0, 0, 0, 0) 0%,
              rgba(0, 0, 0, 0) 80%,
              rgba(0, 0, 0, 0.3) 95%,
              rgba(0, 0, 0, 0.7) 100%);
          pointer-events: none;
        }

        .change-photo-btn {
          position: absolute;
          top: 16px;
          right: 16px;
          z-index: 30;
          background: rgba(0, 0, 0, 0.6);
          border: 1px solid rgba(34, 211, 238, 0.5);
          border-radius: 50%;
          padding: 12px;
          cursor: pointer;
          transition: all 0.3s ease;
          pointer-events: auto;
        }

        .change-photo-btn:hover {
          background: rgba(0, 0, 0, 0.8);
          border-color: #22d3ee;
        }

        .change-photo-btn span {
          font-size: 20px;
          transition: transform 0.3s ease;
          display: block;
        }

        .change-photo-btn:hover span {
          transform: scale(1.1);
        }

        .pc-user-info {
          position: absolute;
          bottom: 20px;
          left: 20px;
          right: 20px;
          z-index: 2;
          display: flex;
          align-items: center;
          justify-content: space-between;
          background: rgba(255, 255, 255, 0.1);
          backdrop-filter: blur(30px);
          border: 1px solid rgba(255, 255, 255, 0.1);
          border-radius: 15px;
          padding: 12px 14px;
          pointer-events: auto;
        }

        .pc-user-details {
          display: flex;
          align-items: center;
          gap: 12px;
        }

        .pc-mini-avatar {
          width: 48px;
          height: 48px;
          border-radius: 50%;
          overflow: hidden;
          border: 1px solid rgba(255, 255, 255, 0.1);
          flex-shrink: 0;
        }

        .pc-mini-avatar img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          border-radius: 50%;
        }

        .pc-user-text {
          display: flex;
          align-items: flex-start;
          flex-direction: column;
          gap: 6px;
        }

        .pc-handle {
          font-size: 14px;
          font-weight: 600;
          color: rgba(255, 255, 255, 0.9);
          line-height: 1;
        }

        .pc-status {
          font-size: 14px;
          color: rgba(255, 255, 255, 0.7);
          line-height: 1;
        }

        .pc-contact-btn {
          border: 1px solid rgba(255, 255, 255, 0.1);
          border-radius: 8px;
          padding: 8px 16px;
          font-size: 14px;
          font-weight: 600;
          color: rgba(255, 255, 255, 0.9);
          cursor: pointer;
          transition: all 0.2s ease;
          backdrop-filter: blur(10px);
          background: none;
        }

        .pc-contact-btn:hover {
          border-color: rgba(255, 255, 255, 0.4);
          transform: translateY(-1px);
        }

        .pc-content {
          max-height: 100%;
          overflow: hidden;
          text-align: center;
          position: relative;
          transform: translate3d(calc(var(--pointer-from-left) * -6px + 3px), calc(var(--pointer-from-top) * -6px + 3px), 0.1px) !important;
          z-index: 5;
          mix-blend-mode: luminosity;
        }

        .pc-details {
          width: 100%;
          position: absolute;
          top: 3em;
          display: flex;
          flex-direction: column;
        }

        .pc-details h3 {
          font-weight: 700;
          margin: 0;
          font-size: min(5vh, 3em);
          background-image: linear-gradient(135deg, #3b82f6, #1e40af, #374151, #6b7280);
          background-size: 300% 300%;
          -webkit-text-fill-color: transparent;
          background-clip: text;
          -webkit-background-clip: text;
          animation: textShimmer 3s ease-in-out infinite;
          text-shadow: 0 0 20px rgba(59, 130, 246, 0.5);
          filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.8));
        }

        .pc-details p {
          font-weight: 600;
          position: relative;
          top: -12px;
          white-space: nowrap;
          font-size: 18px;
          margin: 0 auto;
          width: min-content;
          background-image: linear-gradient(135deg, #6b7280, #374151, #3b82f6);
          background-size: 200% 200%;
          -webkit-text-fill-color: transparent;
          background-clip: text;
          -webkit-background-clip: text;
          animation: textShimmer 2s ease-in-out infinite reverse;
          filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.8));
        }

        .hidden {
          display: none !important;
        }

        @keyframes textShimmer {
          0%, 100% { background-position: 0% 50%; }
          50% { background-position: 100% 50%; }
        }

        @keyframes glow-bg {
          0% { --bgrotate: 0deg; }
          100% { --bgrotate: 360deg; }
        }

        @keyframes holo-bg {
          0% { background-position: 0 var(--background-y), 0 0, center; }
          100% { background-position: 0 var(--background-y), 90% 90%, center; }
        }
    </style>
</head>
<body>
    <div class="container">
        <input type="file" accept="image/*" class="file-input" id="fileInput">

        <!-- Zone d'upload visible quand pas d'image -->
        <div class="upload-zone" id="uploadZone">
            <div class="upload-content">
                <div class="upload-icon">📷</div>
                <div class="upload-text">CLIQUEZ ICI</div>
                <div class="upload-text">POUR VOTRE PHOTO</div>
                <div class="upload-subtext">Fond noir supprimé automatiquement</div>
            </div>
        </div>

        <!-- Indicateur de traitement -->
        <div class="processing-overlay hidden" id="processingOverlay">
            <div class="processing-content">
                <div class="spinner"></div>
                <div class="processing-text">Suppression du fond noir...</div>
                <div class="processing-subtext">Optimisation pour effet 3D transparent</div>
            </div>
        </div>

        <div class="pc-card-wrapper" id="cardWrapper">
            <section class="pc-card" id="card">
                <div class="pc-inside"></div>
                <div class="pc-shine"></div>
                <div class="pc-glare"></div>
                
                <div class="pc-content pc-avatar-content">
                    <img class="avatar hidden" id="avatar" alt="Avatar" loading="lazy">
                    
                    <!-- Bouton pour changer l'image quand elle existe -->
                    <div class="change-photo-btn hidden" id="changePhotoBtn" title="Changer la photo">
                        <span>📸</span>
                    </div>
                    
                    <div class="pc-user-info">
                        <div class="pc-user-details">
                            <div class="pc-mini-avatar">
                                <img id="miniAvatar" src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='48' height='48' viewBox='0 0 48 48'%3E%3Ccircle cx='24' cy='24' r='24' fill='%23374151'/%3E%3Ctext x='24' y='30' text-anchor='middle' fill='white' font-size='16'%3E👤%3C/text%3E%3C/svg%3E" alt="Mini avatar" loading="lazy">
                            </div>
                            <div class="pc-user-text">
                                <div class="pc-handle">Founder BIENAX®</div>
                                <div class="pc-status">Innovation Wellness</div>
                            </div>
                        </div>
                        <button class="pc-contact-btn" onclick="handleContactClick()">
                            Investir dans le projet
                        </button>
                    </div>
                </div>
                
                <div class="pc-content">
                    <div class="pc-details">
                        <h3>BIENAX®</h3>
                        <p>Innovation • Wellness • Future</p>
                    </div>
                </div>
            </section>
        </div>
    </div>

    <script>
        // Variables globales
        let currentAvatarUrl = '';
        let processedImageUrl = '';
        let animationHandlers = null;
        let rafId = null;

        // Configuration
        const ANIMATION_CONFIG = {
            SMOOTH_DURATION: 600,
            INITIAL_DURATION: 1500,
            INITIAL_X_OFFSET: 70,
            INITIAL_Y_OFFSET: 60,
            DEVICE_BETA_OFFSET: 20,
        };

        // Fonctions utilitaires
        const clamp = (value, min = 0, max = 100) => Math.min(Math.max(value, min), max);
        const round = (value, precision = 3) => parseFloat(value.toFixed(precision));
        const adjust = (value, fromMin, fromMax, toMin, toMax) =>
            round(toMin + ((toMax - toMin) * (value - fromMin)) / (fromMax - fromMin));
        const easeInOutCubic = (x) => x < 0.5 ? 4 * x * x * x : 1 - Math.pow(-2 * x + 2, 3) / 2;

        // Suppression du fond noir
        function removeBlackBackground(imageUrl) {
            return new Promise((resolve) => {
                const canvas = document.createElement('canvas');
                const ctx = canvas.getContext('2d');
                const img = new Image();
                
                img.onload = () => {
                    canvas.width = img.width;
                    canvas.height = img.height;
                    
                    // Dessiner l'image
                    ctx.drawImage(img, 0, 0);
                    
                    // Obtenir les données de l'image
                    const imageData = ctx.getImageData(0, 0, canvas.width, canvas.height);
                    const data = imageData.data;
                    
                    // Suppression spécifique du fond noir
                    for (let i = 0; i < data.length; i += 4) {
                        const r = data[i];
                        const g = data[i + 1];
                        const b = data[i + 2];
                        
                        // Détection très précise du noir (avec petite tolérance pour compression)
                        const isBlack = r < 15 && g < 15 && b < 15;
                        
                        // Si c'est noir, le rendre complètement transparent
                        if (isBlack) {
                            data[i + 3] = 0; // Alpha = 0 (transparent)
                        }
                    }
                    
                    // Remettre les données modifiées
                    ctx.putImageData(imageData, 0, 0);
                    
                    // Retourner l'image avec fond noir supprimé
                    resolve(canvas.toDataURL('image/png'));
                };
                
                img.crossOrigin = 'anonymous';
                img.src = imageUrl;
            });
        }

        // Gestion du fichier uploadé
        async function handleFileUpload(event) {
            const file = event.target.files[0];
            if (file) {
                const processingOverlay = document.getElementById('processingOverlay');
                const uploadZone = document.getElementById('uploadZone');
                const avatar = document.getElementById('avatar');
                const changePhotoBtn = document.getElementById('changePhotoBtn');

                processingOverlay.classList.remove('hidden');
                
                // Réinitialiser complètement les états
                currentAvatarUrl = '';
                processedImageUrl = '';
                
                const reader = new FileReader();
                reader.onload = async (e) => {
                    const originalImage = e.target.result;
                    
                    try {
                        // Supprimer spécifiquement le fond noir
                        const processedImage = await removeBlackBackground(originalImage);
                        currentAvatarUrl = originalImage;
                        processedImageUrl = processedImage;
                        
                        // Mettre à jour l'interface
                        avatar.src = processedImage;
                        avatar.classList.remove('hidden');
                        miniAvatar.src = processedImage;
                        uploadZone.classList.add('hidden');
                        changePhotoBtn.classList.remove('hidden');
                        
                    } catch (error) {
                        console.log('Erreur lors du traitement:', error);
                        currentAvatarUrl = originalImage;
                        processedImageUrl = originalImage; // Fallback vers l'image originale
                        
                        avatar.src = originalImage;
                        avatar.classList.remove('hidden');
                        miniAvatar.src = originalImage;
                        uploadZone.classList.add('hidden');
                        changePhotoBtn.classList.remove('hidden');
                    }
                    
                    processingOverlay.classList.add('hidden');
                };
                reader.readAsDataURL(file);
            }
        }

        // Déclenchement de l'upload
        function triggerFileUpload() {
            const fileInput = document.getElementById('fileInput');
            fileInput.value = '';
            fileInput.click();
        }

        // Animation et effets 3D
        function initAnimationHandlers() {
            const updateCardTransform = (offsetX, offsetY, card, wrap) => {
                const width = card.clientWidth;
                const height = card.clientHeight;

                const percentX = clamp((100 / width) * offsetX);
                const percentY = clamp((100 / height) * offsetY);

                const centerX = percentX - 50;
                const centerY = percentY - 50;

                const properties = {
                    "--pointer-x": `${percentX}%`,
                    "--pointer-y": `${percentY}%`,
                    "--background-x": `${adjust(percentX, 0, 100, 35, 65)}%`,
                    "--background-y": `${adjust(percentY, 0, 100, 35, 65)}%`,
                    "--pointer-from-center": `${clamp(Math.hypot(percentY - 50, percentX - 50) / 50, 0, 1)}`,
                    "--pointer-from-top": `${percentY / 100}`,
                    "--pointer-from-left": `${percentX / 100}`,
                    "--rotate-x": `${round(-(centerX / 5))}deg`,
                    "--rotate-y": `${round(centerY / 4)}deg`,
                };

                Object.entries(properties).forEach(([property, value]) => {
                    wrap.style.setProperty(property, value);
                });
            };

            const createSmoothAnimation = (duration, startX, startY, card, wrap) => {
                const startTime = performance.now();
                const targetX = wrap.clientWidth / 2;
                const targetY = wrap.clientHeight / 2;

                const animationLoop = (currentTime) => {
                    const elapsed = currentTime - startTime;
                    const progress = clamp(elapsed / duration);
                    const easedProgress = easeInOutCubic(progress);

                    const currentX = adjust(easedProgress, 0, 1, startX, targetX);
                    const currentY = adjust(easedProgress, 0, 1, startY, targetY);

                    updateCardTransform(currentX, currentY, card, wrap);

                    if (progress < 1) {
                        rafId = requestAnimationFrame(animationLoop);
                    }
                };

                rafId = requestAnimationFrame(animationLoop);
            };

            const cancelAnimation = () => {
                if (rafId) {
                    cancelAnimationFrame(rafId);
                    rafId = null;
                }
            };

            return { updateCardTransform, createSmoothAnimation, cancelAnimation };
        }

        // Gestionnaires d'événements pour l'animation
        function handlePointerMove(event) {
            const card = document.getElementById('card');
            const wrap = document.getElementById('cardWrapper');

            if (!card || !wrap || !animationHandlers) return;

            const rect = card.getBoundingClientRect();
            animationHandlers.updateCardTransform(
                event.clientX - rect.left,
                event.clientY - rect.top,
                card,
                wrap
            );
        }

        function handlePointerEnter() {
            const card = document.getElementById('card');
            const wrap = document.getElementById('cardWrapper');

            if (!card || !wrap || !animationHandlers) return;

            animationHandlers.cancelAnimation();
            wrap.classList.add("active");
            card.classList.add("active");
        }

        function handlePointerLeave(event) {
            const card = document.getElementById('card');
            const wrap = document.getElementById('cardWrapper');

            if (!card || !wrap || !animationHandlers) return;

            animationHandlers.createSmoothAnimation(
                ANIMATION_CONFIG.SMOOTH_DURATION,
                event.offsetX,
                event.offsetY,
                card,
                wrap
            );
            wrap.classList.remove("active");
            card.classList.remove("active");
        }

        // Initialisation
        document.addEventListener('DOMContentLoaded', function() {
            // Initialiser les gestionnaires d'animation
            animationHandlers = initAnimationHandlers();

            // Éléments DOM
            const fileInput = document.getElementById('fileInput');
            const uploadZone = document.getElementById('uploadZone');
            const changePhotoBtn = document.getElementById('changePhotoBtn');
            const card = document.getElementById('card');
            const wrap = document.getElementById('cardWrapper');

            // Event listeners
            fileInput.addEventListener('change', handleFileUpload);
            uploadZone.addEventListener('click', triggerFileUpload);
            changePhotoBtn.addEventListener('click', triggerFileUpload);

            // Animation events
            card.addEventListener('pointerenter', handlePointerEnter);
            card.addEventListener('pointermove', handlePointerMove);
            card.addEventListener('pointerleave', handlePointerLeave);

            // Animation initiale
            if (wrap && card && animationHandlers) {
                const initialX = wrap.clientWidth - ANIMATION_CONFIG.INITIAL_X_OFFSET;
                const initialY = ANIMATION_CONFIG.INITIAL_Y_OFFSET;

                animationHandlers.updateCardTransform(initialX, initialY, card, wrap);
                animationHandlers.createSmoothAnimation(
                    ANIMATION_CONFIG.INITIAL_DURATION,
                    initialX,
                    initialY,
                    card,
                    wrap
                );
            }
        });
    </script>
</body>
</html>
