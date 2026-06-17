# Kivoti - Datenmodell

## Entities
User
Food
DiaryEntry
WeightEntry
WaterEntry
### User
- id
- name
- birthDate
- gender
- height
- targetWeight
- activityLevel
- goal
### Food
- id
- name
- calories
- protein
- carbohydrates
- fat
- saturated fatty acids
- sugar
- portionName
- portionWeight
- barcode
- source
- fiber
- salt
### DiaryEntry
- id
- userId
- foodId
- date
- mealType
- amount
### WeightEntry
- id
- userId
- date
- weight
### WaterEntry
- id
- userId
- date
- amount