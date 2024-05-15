<template>
    <div>
        <link
            rel="stylesheet"
            href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@24,400,0,0"
        />
        <div class="transition">
            <div class="info-discount">
                Sign up and get 20% off to your first order.
            </div>
            <a href="#"> Sign Up Now</a>
            <span class="material-symbols-outlined close-btn"> close </span>
        </div>
        <div class="header-container">
            <div class="logo">SHOP.CO</div>
            <div class="nav-header">
                <div>Shop</div>
                <div>One Sale</div>
                <div>New Arrivals</div>
                <div>Brands</div>
            </div>
            <div class="nav-search">
                <span class="material-symbols-outlined search-icon">
                    search
                </span>
                <input
                    class="text-search"
                    placeholder="Search for products..."
                />
            </div>
            <div class="cart-and-person">
                <span class="material-symbols-outlined"> shopping_cart </span>
                <span class="material-symbols-outlined"> account_circle </span>
            </div>
        </div>
    </div>
</template>

<script>
export default {};
</script>

<style scoped>
.transition {
    width: 100%;
    height: 38px;
    background-color: black;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;

    /* border: 1px solid red; */
}
.info-discount {
    font-size: 14px;
    font-weight: 400;
    line-height: 18.9px;
    text-align: left;
    font-family: 'Satoshi', sans-serif;
    font-size: 14px;
    font-weight: 400;
    line-height: 18.9px;
    text-align: left;
}
a {
    color: white;
    /* font-family: Satoshi; */
    font-size: 14px;
    font-weight: 500;
    line-height: 18.9px;
    text-align: left;
    margin-left: 3px;
}
.close-btn {
    position: absolute;
    right: 0;
    cursor: pointer;
    font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
    margin-right: 100px;
    justify-items: right;
}
.header-container {
    width: 100%;
    height: 96px;
    /* border: 1px solid blue; */
    display: flex;
    justify-content: left;
    align-items: center;
    padding: 0px 100px;
}
.logo {
    font-family: 'Integral CF', sans-serif;
    font-size: 32px;
    letter-spacing: -0.09em;
    font-weight: 800;
    line-height: 38.4px;
    text-align: left;
    margin-right: 50px;
    cursor: pointer;
}
.nav-header {
    display: flex;
    font-family: 'Satoshi', sans-serif;
    font-size: 16px;
    font-weight: 400;
    line-height: 21.6px;
    text-align: left;
    gap: 50px;
    margin-right: 40px;
}
.nav-search {
    width: 577px;
    height: 48px;
    border-radius: 25px;
    display: flex;
    justify-items: center;
    align-items: center;
    background-color: #f0f0f0;
    /* padding-top: 12px; */
    padding-left: 20px;
    margin-right: 40px;
}
.text-search {
    border: 1px solid transparent;
    width: 90%;
    padding: 5px 0px;
    outline: none;
    background-color: #f0f0f0;
    margin-left: 12px;
    opacity: 60%;
    font-family: 'Satoshi', sans-serif;
    font-size: 16px;
    font-weight: 400;
    line-height: 21.6px;
    text-align: left;
}
.search-icon {
    opacity: 60%;
}
.cart-and-person {
    /* width: 577px;
    height: 48px; */
    display: flex;
    gap: 15px;
    justify-items: center;
    /* align-items: right; */
    /* border: 1px solid red; */
}
</style>
