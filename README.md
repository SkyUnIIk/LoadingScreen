# LoadingScreen

    <!-- MUSIC SCRIPT -->
    <!-- To activate simply add a .OGG to the songs folder and it will automatically work, the more songs you add the more random things become :) -->
    <!-- Adding copyrighted music is illegal as you will be redistributing from the server this is hosted from, this means that you will be held liable -->
    
	<?php
	
    $dir = "songs/";
    $song = scandir($dir);
    $i = rand(2, sizeof($song)-1); 

    echo "<audio class='audio' autoplay autobuffer='autobuffer'>";
    echo "<source type='audio/ogg' src='songs/" . $song[$i] . "'>";
	echo "</audio>"
	
	?>
    
    <script type="text/javascript" src="scripts/main.js"></script><!-- Script to get downloads, map, players, game mode and sort out the loading bar -->
	
	</body><!-- Closes off the HTML Document -->
</html>
