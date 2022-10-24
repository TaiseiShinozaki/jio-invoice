<template>
    <v-sheet class="pageback">
        <v-container fluid>
            <v-row>
                <v-col cols="12"><TransactionSection /></v-col>
            </v-row>
            <v-row>
                <v-col cols="12"><TaxProcessing /></v-col>
            </v-row>
            <v-row>
                <v-col cols="12"><DepositAccount /></v-col>
            </v-row>
            <v-row>
                <v-col cols="12"><ClosingDate /></v-col>
            </v-row>
            <v-row>
                <v-col cols="12"><RecoveryCycleMonth /></v-col>
            </v-row>
        </v-container>
        
    </v-sheet>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'
import RecoveryCycleMonth from '../molecules/RecoveryCycleMonth.vue';
import ClosingDate from '../molecules/ClosingDate.vue';
import DepositAccount from '../molecules/DepositAccount.vue';
import TaxProcessing from '../molecules/TaxProcessing.vue';
import TransactionSection from '../molecules/TransactionSection.vue';

@Component({ components: { TransactionSection, TaxProcessing, DepositAccount, ClosingDate, RecoveryCycleMonth }})
export default class CustomerRegisterForm extends Vue {
//登録処理など記述していくのか？
}
</script>
