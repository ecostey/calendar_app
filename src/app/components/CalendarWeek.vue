<template>
    <div id="calendar-week" class="container">
        <div class="columns is-mobile">
            <div class="day column">
                <div class="day-banner has-text-white has-text-centered">Mon</div>
                <div class="day-details">
                    <div class="day-number">1</div>
                    <div class="day-event" style="background-color: rgb(153, 255, 153)">
                        <div>
                            <span class="has-text-centered details">Get Groceries</span>
                            <div class="has-text-centered icons"><i class="fa fa-pencil-square edit-icon"></i>
                                <i class="fa fa-trash-o delete-icon"></i>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="day column">
                <div class="day-banner has-text-white has-text-centered">Tue</div>
                <div class="day-details">
                    <div class="day-number">2</div>
                </div>
            </div>
            <div class="day column">
                <div class="day-banner has-text-white has-text-centered">Wed</div>
                <div class="day-details">
                    <div class="day-number">3</div>
                </div>
            </div>
            <div class="day column">
                <div class="day-banner has-text-white has-text-centered">Thu</div>
                <div class="day-details">
                    <div class="day-number">4</div>
                </div>
            </div>
            <div class="day column">
                <div class="day-banner has-text-white has-text-centered">Fri</div>
                <div class="day-details">
                    <div class="day-number">5</div>
                    <div class="day-event" style="background-color: rgb(255, 153, 153)">
                        <div>
                            <span class="has-text-centered details">Friday dinner/drinks</span>
                            <div class="has-text-centered icons"><i class="fa fa-pencil-square edit-icon"></i>
                                <i class="fa fa-trash-o delete-icon"></i>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="day column">
                <div class="day-banner has-text-white has-text-centered">Sat</div>
                <div class="day-details">
                    <div class="day-number">6</div>
                </div>
            </div>
            <div class="day column">
                <div class="day-banner has-text-white has-text-centered">Sun</div>
                <div class="day-details">
                    <div class="day-number">7</div>
                </div>
            </div>
        </div>
    </div>
</template>


<script>
    import { store } from '../store.js';
    import CalendarDay from './CalendarDay.vue';

    export default {
        name: 'CalendarWeek',
        data () {
            return {
                sharedState: store.state
            }
        },
        components: {
            CalendarDay
        }
    }
</script>


<style lang="scss" scoped>
    #calendar-week {
        margin-bottom: 50px;

        .column {
            padding: 0 0 0 0;
        }
    }
</style>