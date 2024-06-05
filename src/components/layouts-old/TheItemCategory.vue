<template>
    <div class="category-style">
        <div class="title">BROWSE BY DRESS STYLE</div>
        <div class="item-category-01">
            <div class="casual">
                <div class="overlay">
                    <p>Casual</p>
                </div>
            </div>
            <div class="formal">
                <div class="overlay">
                    <p>Formal</p>
                </div>
            </div>
        </div>
        <div class="item-category-02">
            <div class="party">
                <div class="overlay">
                    <p>Party</p>
                </div>
            </div>
            <div class="gym">
                <div class="overlay">
                    <p>Gym</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.category-style {
    height: fit-content;
    background-color: #f0f0f0;
    padding: 80px 0px;
    margin: 0px 100px;
    border-radius: 30px;
}
.title {
    /* margin-top: 72px; */
    font-family: 'Integral CF', sans-serif;
    letter-spacing: -0.07em;
    font-size: 48px;
    font-weight: 800;
    line-height: 57.6px;
    text-align: center;
}
.item-category-01 {
    margin-top: 60px;
    padding: 0px 50px;
    display: flex;
    gap: 30px;
}
.casual {
    cursor: pointer;
    width: 35%;
    height: 289px;
    border-radius: 30px;
    /* border: 1px solid black; */
    background-image: url('../../assets/items/style01.png');
    /* background-position: center; */
    background-position-x: 60px;
    background-position-y: -150px;
}

.overlay {
    position: absolute;
    margin-top: -20px;
    margin-left: 30px;
    font-family: 'Satoshi', sans-serif;
    font-size: 36px;
    font-weight: 700;
    line-height: 48.6px;
    text-align: left;
}
.formal {
    cursor: pointer;
    width: 65%;
    height: 289px;
    /* border: 1px solid black; */
    border-radius: 15px;
    background-size: 130%;
    background-position: center;
    background-position-x: 120px;
    /* background-position-y: 0px; */
    /* background-repeat: no-repeat; */
    background-image: url('../../assets/items/style02.png');
}
.item-category-02 {
    margin-top: 30px;
    padding: 0px 50px;
    display: flex;
    gap: 30px;
}
.party {
    width: 65%;
    height: 289px;
    /* border: 1px solid black; */
    border-radius: 15px;
    background-position: center;
    background-image: url('../../assets/items/style03.png');
    cursor: pointer;
}
.gym {
    cursor: pointer;
    /* border: 1px solid black; */
    width: 35%;
    height: 289px;
    border-radius: 15px;
    background-image: url('../../assets/items/style04.png');
    background-size: cover;
    /* transform-origin: top; */
    background-position: center;
}
@media (max-width: 820px) {
    .category-style {
        padding: 60px 0px;
        margin: 0px 25px;
    }
    .item-category-01 {
        flex-direction: column;
        padding: 0px 20px;
    }
    .casual {
        width: 100%;
        height: 200px;
    }
    .formal {
        width: 100%;
        height: 200px;
    }
    .item-category-02 {
        flex-direction: column;
        padding: 0px 20px;
    }
    .party {
        width: 100%;
        height: 200px;
    }
    .gym {
        width: 100%;
        height: 200px;
    }
}
</style>
