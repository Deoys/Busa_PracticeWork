<script setup>
import TradingPages from './Trading.vue'
import BotRowPages from './BotRow.vue'
import BotColumPages from './BotColum.vue'
import { VueElement } from 'vue'
</script>

<template>
    <div class="infoNavBlock">
            <div class="linkNav">
                <a href="#" class="linkPage">Все счета</a>
                <span>></span>
                <a href="#" class="linkPage">Главный счет</a>
                <span>></span>
                <a href="#" class="linkPage">Боты</a>
            </div>
            <div class="InfoBlock">
                <h2>Боты</h2>
                <div class="addBotButton">
                    <input type="button" value="+" id="AddBot">
                    <label for="AddBot" class="AddBotLabel">Создать бота</label>
                </div>
            </div>
        </div>
        <div id="chartContainer">
            <TradingPages/>
        </div>
        <div class="navBarCur">
            <div class="symbol">
                <div class="CurrTab">
                    <div class="firtPoint">
                    <input type="radio" name="CurrTab" id="All" checked>
                    <label for="All">Все</label>

                    <input type="radio" name="CurrTab" id="ANC">
                    <label for="ANC">ANC/USDT</label>
                    </div>

                    <input type="radio" name="CurrTab" id="BNB">
                    <label for="BNB">BNB/USDT</label>

                    <input type="radio" name="CurrTab" id="BTC">
                    <label for="BTC">BTC/USDT</label>

                    <input type="radio" name="CurrTab" id="ETH">
                    <label for="ETH">ETH/USDT</label>

                    <input type="radio" name="CurrTab" id="WAVES">
                    <label for="WAVES">WAVES/USDT</label>

                    <input type="radio" name="CurrTab" id="FTM">
                    <label for="FTM">FTM/USDT</label>

                    <input type="radio" name="CurrTab" id="XRP">
                    <label for="XRP">XRP/USDT</label>

                    <input type="radio" name="CurrTab" id="ADA">
                    <label for="ADA">ADA/USDT</label>

                    <input type="radio" name="CurrTab" id="DOGE">
                    <label for="DOGE">DOGE/USDT</label>
                </div>
                <select name="OtheCurr" id="OtheCurr">
                    <option value="0">другие пары</option>
                </select>
            </div>
            <div class="BotViewSellect">
                <button class="Botcol" @click="viewTabel('Colum')">
                    <img src="../assets/materials/main/i-cols-layout.png" alt="">
                </button>
                <button class="Botlist" @click="viewTabel('Row')">
                    <img src="../assets/materials/main/i-list-layout.png" alt="">
                </button>
            </div>
        </div>
        <div class="BotList" ref="Bot">
            <div class="Bot BotRow">
            <BotRowPages/>
            </div>
            <div class="Bot Colum BotColum">
            <BotColumPages/>
            </div>
        </div>
        <button class="AddBotMain">
            <svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M6.99998 0.333008C7.46022 0.333008 7.83331 0.706104 7.83331 1.16634V6.16634H12.8333C13.2936 6.16634 13.6666 6.53944 13.6666 6.99967C13.6666 7.45991 13.2936 7.83301 12.8333 7.83301H7.83331V12.833C7.83331 13.2932 7.46022 13.6663 6.99998 13.6663C6.53974 13.6663 6.16665 13.2932 6.16665 12.833V7.83301H1.16665C0.706409 7.83301 0.333313 7.45991 0.333313 6.99967C0.333313 6.53944 0.706409 6.16634 1.16665 6.16634H6.16665V1.16634C6.16665 0.706104 6.53974 0.333008 6.99998 0.333008Z" fill="#366AF3"/>
            </svg>
            Добавить бота
        </button>
</template>

<script>
    export default {
        methods:{
            viewTabel:function (message) {
                if(message == 'Colum'){
                    document.querySelector(".BotRow").style.display = 'none';
                    document.querySelector(".BotColum").style.display = 'flex';
                }if(message == 'Row'){
                    document.querySelector(".BotRow").style.display = 'flex';
                    document.querySelector(".BotColum").style.display = 'none';
                }
            }
        }
    }
</script>
