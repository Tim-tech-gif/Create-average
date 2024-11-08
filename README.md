# Create-average
fn gen_shipments(mut shipments: Vec&lt;u32>) -> Vec&lt;u32> {     let total: u32 = shipments.iter().sum();     let average = total as i32 / shipments.len() as i32;      let mut adjustments: Vec&lt;i32> = shipments.iter().map(|&amp;x| x as i32 - average).collect();      // Перевіримо, чи загальний залишок не більше нуля (щоб врівноважити).     let excess: i32
