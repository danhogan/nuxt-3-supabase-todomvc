<template>
  <div>
    <NuxtWelcome />
  </div>
</template>

<script setup>
import { createClient } from '@supabase/supabase-js/dist/main/index'

const { supabaseUrl, supabasePublicKey} = useRuntimeConfig();

const supabase = createClient(supabaseUrl, supabasePublicKey)
</script>