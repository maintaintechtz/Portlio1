 
.btn-box .btn{
    position: relative;
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width:15rem ;
    height:100% ;
    background: var(--main-color);
    border: .2rem  solid var(--main-color);
    border-radius: .8rem;
    font-size: 1.9rem;
    font-weight: 600;
    letter-spacing: .1rem;
    color:var(--bg-color);
    z-index: 1;
    overflow: hidden;
    transition: 0.5s;
    
}
.btn-box .btn:nth-child(2){
    background: transparent;
    color: var(--main-color);
}
.btn-box .btn:nth-child(2):hover{
    color:var(--bg-color)

}
.btn-box .btn:nth-child(2)::before{
    background:var(--main-color)
}
.btn-box .btn::before{
    content:'';
    position: absolute;
    top: 0;
    left: 0;
    width: 0;
    height:100%;
    background:var(--main-color);
    z-index: -1;
    transition: 0.5s;


}
.btn-box .btn:hover::before{
    width: 100%;  

}