<template>
    <v-card class="mx-auto" max-width="40rem" outlined>
        <v-list-item three-line>
            <v-list-item-content>

                <!-- Upper Tag -->
                <div class="text-overline mb-4">
                    {{ upperTag }}
                </div>

                <!-- Title -->
                <v-list-item-title class="text-h5 mb-1">
                    {{ title }}
                </v-list-item-title>

                <!-- Subtitle -->
                <v-list-item-subtitle>
                    {{ subtitle }}
                </v-list-item-subtitle>

            </v-list-item-content>

            <!-- <v-list-item-avatar tile size="80" color="grey"></v-list-item-avatar> -->
        </v-list-item>

        <v-card-actions>
            <v-btn outlined rounded text :to=buttonRoute>
                {{ buttonText }}
            </v-btn>
        </v-card-actions>
    </v-card>
</template>

<script>
export default {
    name: 'Card',
    props: {
        upperTag: String,
        title: String,
        subtitle: String,
        buttonText: String,
        buttonRoute: String
    }
}
</script>