<title>soooongs</title>
<style>
    :global(body) {
        margin: 0;
        padding: 0;
        background: #1a1a1a;
        overflow: hidden;
    }

    .container {
        position: relative;
        width: 100%;
        height: 100vh;
        background: #2a2a2a;
    }

    .background {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        overflow: hidden;
    }

    @keyframes float {
        0%, 100% {
            transform: translate(0, 0);
        }
        33% {
            transform: translate(50px, -50px);
        }
        66% {
            transform: translate(-30px, 30px);
        }
    }

    .orb {
        position: absolute;
        border-radius: 50%;
        background: rgba(100, 150, 255, 0.3);
        filter: blur(40px);
    }

    .orb1 {
        width: 300px;
        height: 300px;
        top: 10%;
        left: 15%;
        animation: float 8s infinite ease-in-out;
        animation-delay: 0s;
    }

    .orb2 {
        width: 250px;
        height: 250px;
        top: 60%;
        left: 70%;
        animation: float 10s infinite ease-in-out;
        animation-delay: 2s;
    }

    .orb3 {
        width: 200px;
        height: 200px;
        top: 30%;
        right: 10%;
        animation: float 12s infinite ease-in-out;
        animation-delay: 4s;
    }

    .title {
        position: relative;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
        width: 100%;
        height: 100vh;
        gap: 2rem;
        z-index: 1;
    }

    .welcome {
        color: white;
        font-family: 'Courier New', monospace;
        font-size: 24px;
        margin: 0;
    }

    .soooongs {
        color: white;
        font-family: 'Brush Script MT', cursive;
        font-size: 120px;
        margin: 0;
        font-weight: normal;
    }

    .login-button {
        background: transparent;
        color: white;
        font-family: 'Courier New', monospace;
        font-size: 18px;
        padding: 15px 40px;
        border: 2px solid white;
        border-radius: 8px;
        cursor: pointer;
        transition: all 0.3s ease;
    }

    .login-button:hover {
        background: white;
        color: #2a2a2a;
    }

    .login-text {
        position: absolute;
        top: 30px;
        left: 30px;
        color: white;
        font-family: 'Courier New', monospace;
        font-size: 18px;
        margin: 0;
    }
</style>

<div class="container">
    <div class="background">
        <div class="orb orb1"></div>
        <div class="orb orb2"></div>
        <div class="orb orb3"></div>
    </div>
    
    <p class="login-text">login</p>
    
    <div class="title">
        <h1 class="welcome">welcome to</h1>
        <p class="soooongs">Soooongs</p>
        <button class="login-button">login w spotify</button>
    </div>
</div>