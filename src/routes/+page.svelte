<script>
	import { focusedHeader } from '../store.js';
	focusedHeader.set('h1');
</script>

	<div class="home">
        <div class="section-1">
            <img style="align-items: start" src="https://upload.wikimedia.org/wikipedia/commons/b/b2/Kanchi-Maha-Periyava.jpg" alt="Kanchi Mahaperiyavar"/>
            <div>Astro Acharya</div>
            <img src="https://upload.wikimedia.org/wikipedia/commons/e/ef/Ganesha_%2828862909620%29.jpg" alt="Ucchista Maha Ganapathi"/>
        </div>        
        <div class="section-2">Welcome to Astro Acharya, our Vedic Astrology Hub, where ancient wisdom meets modern solutions.</div>        
    </div>

<style>
    .section-1 {
        position: relative;
		padding: 0;
		margin: 0;
		display: flex;
		justify-content: space-between;
		align-items: center;
    }

    .section-1 img {
		display: flex;		
		align-items: center;
		padding: 0 0.5rem;
        width: 360px;
        height: 400px;		
	}

    .section-1 div {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;	
        font-family: fantasy;	
        font-size: 2rem;
	}

    .section-2 {
        margin-top: 75px;
        display: flex;
		height: 100%;
		align-items: center;
        justify-content: center;
		padding: 0 0.5rem;	
        font-family: monospace;	
        font-size: 1.5rem;
    }
</style>
