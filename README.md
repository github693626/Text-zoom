# Text-zoom

##載入

      <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.3/jquery.min.js"></script>

##HTML

      <a class="BtnFontZoom" href="#">Text zoom +</a>
      	
      <p class="fontZoom">
      	Test text<br>
      	Test text<br>
      	Test text<br>
      	Test text<br>
      	Test text<br>
      	Test text<br>
      	Test text<br>
      	Test text<br>
      </p>

##CSS

      p{font-size: 18px;line-height: 1.5;}

##JS

      $(function(){
      
      	var _fontSize = 0;
      	var _newSize = 0;
      	var $fontZoom = $(".fontZoom");
      
      	$(".BtnFontZoom").click(function() {
      
      		_fontSize = parseInt($fontZoom.css("font-size"));
      		
      		if( _fontSize <= 18){
      			_newSize = 24;
      		}else if(_fontSize <= 24){
      			_newSize = 28;
      		}else{
      			_newSize = 18;
      		}
      
      		$fontZoom.css("font-size",_newSize);
      		return false;
      		
      	});
      		
      
      });
