# REACT-SLIDER-SLIDER_CRATE-_KARE-_EASILY
INSTALL : npm install react-slick slick-carousel
IMPORT KARE JAHA USE KAR ERAHE HAI 
import "slick-carousel/slick/slick.css"; 
import "slick-carousel/slick/slick-theme.css";


```javascript
import React from "react";
import Slider from "react-slick";
import "slick-carousel/slick/slick.css"; 
import "slick-carousel/slick/slick-theme.css";

function ReactSlickExample() {
  // Settings for React Slick
  const settings = {
    dots: true,              // Show dots indicators below slider
    infinite: true,          // Infinite scrolling
    speed: 500,              // Transition speed
    slidesToShow: 3,         // Number of slides visible
    slidesToScroll: 1,       // Number of slides to scroll at once
    autoplay: true,          // Enable autoplay
    autoplaySpeed: 2000,     // Autoplay speed (2 seconds)
  };

  // Sample Data for Slider
  const images = [
    "https://via.placeholder.com/300x200?text=Slide+1",
    "https://via.placeholder.com/300x200?text=Slide+2",
    "https://via.placeholder.com/300x200?text=Slide+3",
    "https://via.placeholder.com/300x200?text=Slide+4",
    "https://via.placeholder.com/300x200?text=Slide+5",
  ];

  return (
    <div style={{ margin: "20px" }}>
      <h2>React Slick Example</h2>
      <Slider {...settings}>
        {images.map((image, index) => (
          <div key={index}>
            <img src={image} alt={`Slide ${index + 1}`} style={{ width: "100%" }} />
          </div>
        ))}
      </Slider>
    </div>
  );
}

export default ReactSlickExample;
```


Slider Settings:

dots: Slider ke neeche dots dikhata hai (pagination ke liye).
infinite: Slider ko infinite loop me chalata hai.
slidesToShow: Ek baar me kitne slides visible honge.
slidesToScroll: Ek baar me kitne slides scroll honge.
autoplay: Slider ko automatically move karata hai.
autoplaySpeed: Autoplay ka interval (milliseconds me).



## custrom responsive kar sakte hai 
```
responsive: [
  {
    breakpoint: 1024,
    settings: {
      slidesToShow: 3,
      slidesToScroll: 1,
      infinite: true,
      dots: true,
    },
  },
  {
    breakpoint: 600,
    settings: {
      slidesToShow: 2,
      slidesToScroll: 1,
    },
  },
  {
    breakpoint: 480,
    settings: {
      slidesToShow: 1,
      slidesToScroll: 1,
    },
  },
]
```

----
----





