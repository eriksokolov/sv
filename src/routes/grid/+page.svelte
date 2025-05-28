<style>
    .container{
        max-width: 960px;
        margin: 100px auto;
        padding: 10px;
        display:grid;
        grid-template-columns: 1fr 1fr 1fr;
    }
    .item{
        background:steelblue;
        color: #fff;
        font-size: 20px;
        padding: 20px;
        border: skyblue 1px solid;
    }
    .item:nth-of-type(2){
        height: 100px;
        width: 100px;
        justify-self: center;
    }
@media (max-width: 900px){
    .container {
        grid-template-columns: 1fr;
    }
}
</style>
<div class="container">
    <div class="item">item</div>
    <div class="item">item</div>
    <div class="item">item</div>
    <div class="item">item</div>
    <div class="item">item</div>
    <div class="item">item</div>
    <div class="item">item</div>
    <div class="item">item</div>
</div>