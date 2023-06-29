<template>
    <div class="shortInfo">
        <div class="HeaderInfo">
            <div class="headerInfoRow1">
                <div class="leftItem">
                    <div class="linkSerNum">
                        <img src="../assets/materials/main/arrow-up-right-square.png" alt="">
                        <p>#562019</p>
                    </div>
                    <div class="scriptBot">
                        <div class="CheckBoxTougel">
                            <label class="Switch" for="RestartTougel">
                                <input type="checkbox" name="RestartTougel" id="RestartTougel">
                                <span class="demo"></span>
                            </label>
                            <p>Без перезапуска</p>
                        </div>
                        <button class="ActionButton">
                            <img src="../assets/materials/main/play-fill.png" alt="">
                        </button>
                    </div>
                </div>
                <div class="rightIteam">
                    <div class="costCoin">
                        <img src="../assets/materials/main/WAVES.png" alt="">
                        <div class="">1 waves =</div><span>105.63019</span> 
                        <div class="">USDT</div>
                    </div>
                    <div class="setingIcon">
                        <img src="../assets/materials/main/i-gear-fill.png" alt="">
                    </div>
                    <div class="logoCoin">
                        <img src="../assets/materials/main/WAVES.png" alt="">
                        <h3>Waves/usdt</h3>
                    </div>
                </div>
            </div>
            <div class="headerInfoRow2">
                <h2>Бот фиксирующий прибыль после распределения входных точек по завершённым тэйкам </h2>
            </div>
        </div>
        <div class="MetaInfo">
            <div class="OrderInfo">
                <div class="CountOrder">
                    <span>Выставлено</span>
                    <span class="countOrd">2</span>
                    <span>ордера</span>
                    <div class="MenuOrder">
                        <div></div>
                        <div></div>
                        <div></div>
                    </div>
                </div>
                <div class="executedOrder">
                    <span>Исполнен</span>
                    <span class="execut">1</span>
                    <span>ордер</span>
                    <a href="#">история действий</a>
                </div>
            </div>
            <div class="StatusOrder">
                <div class="DailyStatus">
                    <div class="">В текущем цикле:</div>
                    <span><img src="../assets/materials/main/arrow-down-short.png" alt="">64`579.17</span>
                    <div class="">USDT</div>
                    <span>(20.89%)</span>
                </div>
                <div class="GeneralStatus">
                    <div class="">За все 43 дня:</div>
                    <span><img src="../assets/materials/main/arrow-up-short.png" alt="">164`579.17</span>
                    <div class="">USDT</div>
                    <a href="#">статистика</a>
                </div>
            </div>
        </div>
    </div>
    <div class="BalanceBotInfo">
        <div class="balance">
            <div class="">Баланс</div>
            <div class="infoSimbol"><span>0</span>WAVES</div>
        </div>
        <div class="avPrice">
            <div class="">Ср. цена</div>
            <div class="infoSimbol"><span>-</span></div>
        </div>
        <div class="Summ">
            <div class="">Сумма</div>
            <div class="infoSimbol"><span>-</span></div>
        </div>
        <div class="CurrentSumm">
            <div class="">Текущая сумма</div>
            <div class="infoSimbol"><span>-</span>
                <div class="tagSumm">
                    <img src="../assets/materials/main/arrow-down-short.png" alt="">
                    <span>88</span>
                    <div>usdt</div> 
                    <span>(4.37%)</span>
                </div>
            </div>
        </div>
        <div class="ExtraSale">
            <a href="#"><img src="../assets/materials/main/coin.png" alt=""><span>продать</span></a>
        </div>
        <button class="HideActions" @click="CloseAction()">
            <span>скрыть действия</span>
        </button>
    </div>
    <div class="ActionsBot">
        <div class="infActions">
            <div class="boxInfoAction">
                <div class="nameInfo">
                    <span>Entry Point</span>
                </div>
                <div class="ColumnsAction">
                    <div class="rowInfoAct columAct">
                        <div class="numrow">##</div>
                        <div class="pricerow">
                        </div>
                        <div class="Amountrow">
                            <div class="row">
                                <p>Сумма</p>
                            </div>
                        </div>
                        <div class="settingsrow">
                            <div class="row">
                                <p>Настройки</p>
                            </div>
                        </div>
                        <div class="Trigerrow">
                            <div class="row">
                                <p>Триггер</p>
                            </div>
                        </div>
                        <div class="Trailingrow">
                            <div class="row">
                                <p>Trailing</p>
                            </div>
                        </div>
                    </div>
                    <div class="columAct">
                        <div class="numrow">#1</div>
                        <div class="pricerow activ">
                            <div class="row">
                                <p>Цена</p>
                                <img src="../assets/materials/main/check-circle-fill.png" alt="">
                            </div>
                            <p>100 udst</p>
                        </div>
                        <div class="Amountrow activ">
                            <div class="row">
                                <p>Сумма</p>
                                <p>20 waves</p>
                            </div>
                        </div>
                        <div class="Trigerrow">
                            <div class="row">
                                <p>Триггер</p>
                                <p>105 udst</p>
                            </div>
                        </div>
                        <div class="Trailingrow">
                            <div class="row">
                                <p>Trailing</p>
                                <p>2%</p>
                            </div>
                        </div>
                    </div>
                    <div class="columAct">
                        <div class="numrow">#2</div>
                        <div class="pricerow">
                            <div class="row">
                                <p>Цена</p>
                                <img src="../assets/materials/main/pause-circle-fill.png" alt="">
                            </div>
                            <p>90 udst</p>
                        </div>
                        <div class="Amountrow">
                            <div class="row">
                                <p>Сумма</p>
                                <p>20 waves</p>
                            </div>
                        </div>
                        <div class="Trigerrow">
                            <div class="row">
                                <p>Триггер</p>
                                <p>95 udst</p>
                            </div>
                        </div>
                        <div class="Trailingrow">
                            <div class="row">
                                <p>Trailing</p>
                                <p>2%</p>
                            </div>
                        </div>
                    </div>
                    <div class="columAct">
                        <div class="numrow">#3</div>
                        <div class="pricerow">
                            <div class="row">
                                <p>Цена</p>
                                <img src="../assets/materials/main/pause-circle-fill.png" alt="">
                            </div>
                            <p>80 udst</p>
                        </div>
                        <div class="Amountrow">
                            <div class="row">
                                <p>Сумма</p>
                                <p>20 waves</p>
                            </div>
                        </div>
                        <div class="settingsrow">
                            <div class="row">
                                <p>Настройки</p>
                                <p>50%</p>
                            </div>
                        </div>
                        <div class="Trigerrow">
                            <div class="row">
                                <p>Триггер</p>
                                <p>85 udst</p>
                            </div>
                        </div>
                        <div class="Trailingrow">
                            <div class="row">
                                <p>Trailing</p>
                                <p>2%</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="boxInfoAction">
                <div class="nameInfo">
                    <span>Take Profit</span>
                </div>
                <div class="ColumnsAction">
                    <div class="columAct">
                        <div class="numrow">#4</div>
                        <div class="pricerow">
                            <div class="row">
                                <p>Цена</p>
                                <img src="../assets/materials/main/pause-circle-fill.png" alt="">
                            </div>
                            <p>100 udst</p>
                        </div>
                        <div class="Amountrow">
                            <div class="row">
                                <p>Сумма</p>
                                <p>6 waves</p>
                            </div>
                        </div>
                        <div class="settingsrow">
                            <div class="row">
                                <p>Настройки</p>
                                <p>50%</p>
                            </div>
                        </div>
                        <div class="Trigerrow">
                            <div class="row">
                                <p>Триггер</p>
                                <p>-</p>
                            </div>
                        </div>
                        <div class="Trailingrow">
                            <div class="row">
                                <p>Trailing</p>
                                <p>2%</p>
                            </div>
                        </div>
                    </div>
                    <div class="columAct">
                        <div class="numrow">#5</div>
                        <div class="pricerow">
                            <div class="row">
                                <p>Цена</p>
                                <img src="../assets/materials/main/pause-circle-fill.png" alt="">
                            </div>
                            <p>140 udst</p>
                        </div>
                        <div class="Amountrow">
                            <div class="row">
                                <p>Сумма</p>
                                <p>6 waves</p>
                            </div>
                        </div>
                        <div class="settingsrow">
                            <div class="row">
                                <p>Настройки</p>
                                <p>30%</p>
                            </div>
                        </div>
                        <div class="Trigerrow">
                            <div class="row">
                                <p>Триггер</p>
                                <p>120 udst</p>
                            </div>
                        </div>
                        <div class="Trailingrow">
                            <div class="row">
                                <p>Trailing</p>
                                <p>-</p>
                            </div>
                        </div>
                    </div>
                    <div class="columAct">
                        <div class="numrow">#6</div>
                        <div class="pricerow">
                            <div class="row">
                                <p>Цена</p>
                                <img src="../assets/materials/main/pause-circle-fill.png" alt="">
                            </div>
                            <p>150 udst</p>
                        </div>
                        <div class="Amountrow">
                            <div class="row">
                                <p>Сумма</p>
                                <p>6 waves</p>
                            </div>
                        </div>
                        <div class="settingsrow">
                            <div class="row">
                                <p>Настройки</p>
                                <p>30%</p>
                            </div>
                        </div>
                        <div class="Trigerrow">
                            <div class="row">
                                <p>Триггер</p>
                                <p>140 udst</p>
                            </div>
                        </div>
                        <div class="Trailingrow">
                            <div class="row">
                                <p>Trailing</p>
                                <p>-</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="boxInfoAction">
                <div class="nameInfo">
                    <span>Stop Loss</span>
                </div>
                <div class="ColumnsAction">
                    <div class="columAct">
                        <div class="numrow">#7</div>
                        <div class="pricerow">
                            <div class="row">
                                <p>Цена</p>
                                <img src="../assets/materials/main/pause-circle-fill.png" alt="">
                            </div>
                            <p>70 udst</p>
                        </div>
                        <div class="Amountrow">
                            <div class="row">
                                <p>Сумма</p>
                                <p>10 waves</p>
                            </div>
                        </div>
                        <div class="settingsrow">
                            <div class="row">
                                <p>Настройки</p>
                                <p>50%</p>
                            </div>
                        </div>
                        <div class="delayrow">
                            <div class="row">
                                <p>Задержка</p>
                                <p>5 мин</p>
                            </div>
                        </div>
                    </div>
                    <div class="columAct">
                        <div class="numrow">#8</div>
                        <div class="pricerow">
                            <div class="row">
                                <p>Цена</p>
                                <img src="../assets/materials/main/pause-circle-fill.png" alt="">
                            </div>
                            <p>65 udst</p>
                        </div>
                        <div class="Amountrow">
                            <div class="row">
                                <p>Сумма</p>
                                <p>5 waves</p>
                            </div>
                        </div>
                        <div class="settingsrow">
                            <div class="row">
                                <p>Настройки</p>
                                <p>25%</p>
                            </div>
                        </div>
                        <div class="delayrow">
                            <div class="row">
                                <p>Задержка</p>
                                <p>5 мин</p>
                            </div>
                        </div>
                    </div>
                    <div class="columAct">
                        <div class="numrow">#9</div>
                        <div class="pricerow">
                            <div class="row">
                                <p>Цена</p>
                                <img src="../assets/materials/main/pause-circle-fill.png" alt="">
                            </div>
                            <p>60 udst</p>
                        </div>
                        <div class="Amountrow">
                            <div class="row">
                                <p>Сумма</p>
                                <p>5 waves</p>
                            </div>
                        </div>
                        <div class="settingsrow">
                            <div class="row">
                                <p>Настройки</p>
                                <p>25%</p>
                            </div>
                        </div>
                        <div class="delayrow">
                            <div class="row">
                                <p>Задержка</p>
                                <p>5 мин</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
 export default {
    methods:{
        CloseAction:function(){
            if(document.querySelector(".ActionsBot").style.display =='' || document.querySelector(".ActionsBot").style.display == 'block')
            {
                document.querySelector(".ActionsBot").style.display = 'none';
                document.querySelector(".HideActions span").textContent = "показать действия"
                return;
            }
           if(document.querySelector(".ActionsBot").style.display == 'none'){
            document.querySelector(".ActionsBot").style.display = 'block';
            document.querySelector(".HideActions span").textContent = "скрыть действия"
           }
        }
    }
 }
</script>