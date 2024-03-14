
## **Kas ir API?**

        Interfeiss kas ļauj sadarboties front-end un back-end, ļauj veikt pieprasījumus un gūt atpakaļ atbildi parasti JSON formātā.

## **Kā deklarēt mainīgo PHP valodā?**

      $mainiga_nosaukums = “vērtība”;

## **Kādu arhitektūru izmanto Laravel, paskaidro kā tā strādā:**

      Laravel izmanto modulāru arhitektūru, kas ļauj sadalīt darbu mazākās vienībās, kuras var izmantot atsevišķi
      
## **Kas ir ORM, kāpēc to izmanto tīra SQL vietā?**

      ORM ir veids kā pārveidot SQL datus un tabulas programmēšanas valodas objektos vieglākai apstrādei. Ir vieglāk apstrādāt datus kad tie ir objekta formā un glabājas RAM, nevis uz cietā diska.

## **Uzraksti Eloquent ORM pieprasījumu modelim User, kur nepieciešams iegūt visus lietotājus kuriem reitings ir lielāks par 4. Lietotāju tabulas struktūra:**

| Lauks      | Limiti        |
|------------|---------------|
|  username  | VARCHAR(255)  |
|  email     | VARCHAR(255)  |
|  password  | VARCHAR(255)  |
|  rating    | DECIMAL(8, 2) |
| created_at | TIMESTAMP     |
| updated_at | TIMESTAMP     |

    $users = User::where(‘rating’, ‘>’, 4)->get();
