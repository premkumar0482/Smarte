# Smarte
*Smarterp.jsx
import React, {useState} from 'react'
import Style from './smarterp.module.css'
const Smarterp = () => {
    const [Query,setQuery]=useState("");
    let btn=()=>{
        this.demoref.current.style.background="red"
    }
    return (
        <section id={Style.App}>
            <article>
                <div className={Style.Search}>
                    <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAJEAAACRCAMAAAD0BqoRAAAAaVBMVEXm5uYzMzPq6urt7e0oKCgvLy8fHx/w8PArKysjIyPj4+P09PQAAAAcHBxlZWUYGBjc3Nx6enrV1dVQUFBJSUk6OjpcXFxwcHC6urqCgoLMzMyOjo7ExMSUlJSgoKBra2uqqqoQEBBBQUGz3s1yAAAEkElEQVR4nO2a25arKBCGQwEiGjxrPB/y/g85hZqs3j3diZnZkFzwXZnoWvwWP0UBnk4Oh8PhcDgcDofD4XA4HA6Hw6EBoCJcERTeLUbLCbJ6uOTXsiyibm4TeK8oCLOhKmOPcY0vY5k3NRXv03Oqq1hyouE+Xy84i8sxoe8RRLPIZ1qDVIoXeV5KHSz8QxbzOwwFp2bxCfFV3szt7uyk7yImUVNctNYlQRZ5qIdVdQL3gOCoC9qGY+BYOVvuOdoTbFdVPf3eMIiskT7hy2A1SrRHH/v+GGytwo39V5ujXNlYjNIqiBX9OsyB0qweu6Yb5vYkVlE0aGKMYGctSpARFJRvAYJszLnPVvxr02+BogNGyRutRSliKCjZBM2l8jnzlmVRknMpL224/j8saPzeTpRo5xG/2C0UXBnjeTPWfT13USm5H3frLdExwq+BDUmQxV/fvlNTn1AKer4Nso5LoqZNR+SjlazMKNhSPN5borubN7UCGsZZoXsUEkzg3EK/Qe0Tvwp+vQ01Sor0fRjRbql5cwu0tawfvDltS+5tQnJO4sx0kCBRGKKHL057KX3dq3RWRBpP3TCgdevHXQFzNa86givn+a8d/LeIOC+SJ8/AaZ9PdAYw7G3ISnTr0Tb0KFCGEzf0MZGHCw0IUH8UGlVER0W849VYmGP5bVaRSBlRx40hGkbOZnstrHzCjr80HT1yToxaOyw4v76gCDPS2WyO1IqKVxTF5Gx2EfCBinDwkFd8pEz7SFxwrB2veUQnydmgHN3E4BF13Kp6aMZm8xHUMfEe1SLfHr8SPzesqMVVyOFVj37a6wzXbAla+/cK8hu6inxY3f0NKBYY8nCBUfnPS5f/i578WXpstEEvXyhd/jOiwBXGsdFGJ0YW84sRmPHFmyPNQM+xJLewhAxwhaH6AwMIcqwTTPtaQ+uF8OL51EA7hQWkeT2IqI6sDCnW2CS2s/kH2RVXhk+sRNuFEGlru0b3G5EPNxloi6rlZG1LSxerZEl/34pBzTjbVFb2ajYAXYstZj93CkCHHmLX5LaStAEdFCYbOQT/1gS0zlGvrBIASCdr5yQwE4yDzMcEvraJ1/3E9Z0pwOtGeo0lQdq7RUwIV2VTJzSkGhFCP1ae3mBfRr2npXdsvUtoLUrBQNZjEVYW6TDO89BUJdcHNz6bWuxNSKU+u8EoWZMk2kZ5fD0w8pRSntyul6reOjJaFREvtXduAzQZK6LYdqCF+B7L0/5mrD1IRD7IEwY0Be18Kc8bXjXUXw4hIdCnOWuUzNba30WBCEWQZVkCYSj+DIZId0kXi5npruunxAPBZffSoYrKBkAvtyh9wjm3BqPkfVqUxC0JfFCU0puX7Nv7ZwCmm5esTShPwBLAs58qHwKn6TahiE+RBG9MlT8DwR4l2bzvq5I/AXFPlW/++ubOR04oexKQl4+xd5DeJ5RPkURvSeBzonS6TSip8ZPJg2Cq3DoutvcBxxOAbl565bjHMHuqlNPHKNJVZcxlkb1bxxcg6MrI+HcJr0HDz+kyh8PhcDgcDofD4XA4HA6Hw2GVfwBO5zcWkxzZ3AAAAABJRU5ErkJggg==" alt="" />
                    <input type="search" placeholder="Search..." onChange={e=> setQuery(e.target.value)}/>
                </div>
                <div className={Style.Post}>
                    <form action="">
                    <input type="button" value="New Post" />
                    <input type="button" value="Published" />
                    </form>
                </div>
                <div className={Style.Details}>
                    <div className={Style.Title} >Title:     Frontend Developer</div>
                    <div className={Style.Markdown}>
                        <input type="text" />
                    </div>
                    <div className={Style.Publish}>Publish:</div>
                </div>
            </article>
        </section>
    );
}

export default Smarterp


*smarterp.module.css

*{
    padding: 90;
    margin: 0;
    box-sizing: border-box;
}
img{
    height: 20px;
}
#App{
    height: 500px;
    width: 60%;
    border: 2px solid black;
    background-color: wheat;

}
#App>article{
    height: 50px;
    width: 100%;
    border: 2px solid white;
    text-align: center;
}
#App>article>.Search{
    border: 3px solid red;
    height: 50px;
    width: 100%;
}
#App>article>.Post{
    border: 3px solid red;
    height: 50px;
    width: 100%;
}
#App>article>.Details{
    border: 3px solid red;
    height: 350px;
    width: 100%;
    
}
#App>article>.Details>.Title{
    border: 2px solid black;
    height: 100px;
    width: 100%;
}
#App>article>.Details>.Markdown{
    border: 2px solid black;
    height: 100px;
    width: 100%;
}
#App>article>.Details>.Publish{
    border: 2px solid black;
    height: 100px;
    width: 100%;
    
}

