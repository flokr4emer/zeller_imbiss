<script setup>
import { openingHours } from '../js/openingHours';
</script>

<template>
    <table class="table table-borderless table-responsive table-sm small text-muted">
        <tbody v-for="element in openingHours" :key="element.weekDay">
            <tr>
                <th scope="row">{{ element.weekDay }}</th>
                <td>{{ element.opens }} - {{ element.closes }}</td>

            </tr>
        </tbody>
    </table>
</template>

<script>
export default {
    name: "OpeningHoursTableItem"
}
</script>

<style></style>