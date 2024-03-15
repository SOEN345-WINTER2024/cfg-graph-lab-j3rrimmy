Jeremy Rimokh -- 40110746

## CFG Graph
![CFG drawio](https://github.com/SOEN345-WINTER2024/cfg-graph-lab-j3rrimmy/assets/98069409/8da64214-7428-4121-875f-adbe3e0cf315)


### Node Coverage
#### Node Test Requirements
[1][2][3][4][5][6][7][8][9][10][11][12][13][14][15][16][17][18][19][20][21][22]

#### Node Test Paths
[1,2,22][1,3,22][1,4,22][1,5,22][1,6,22][1,7,22][1,8,22][1,9,22][1,10,22][1,11,22][1,12,22][1,13,22][1,14,22][1,15,22][1,16,22][1,17,18,22][1,17,19,22][1,17,20,22][1,17,21,22]

### Edge Coverage
#### Edge Test Requirements 
[1,2][1,3][1,4][1,5][1,6][1,7][1,8][1,9][1,10][1,11][1,12][1,13][1,14][1,15][1,16][1,17][17,18][17,19][17,20][17,21][18,22][19,22][20,22][21,22]
[2,22][3,22][4,22][5,22][6,22][7,22][8,22][9,22][10,22][11,22][12,22][13,22][14,22][15,22][16,22]

#### Edge Test Paths
[1,2,22][1,3,22][1,4,22][1,5,22][1,6,22][1,7,22][1,8,22][1,9,22][1,10,22][1,11,22][1,12,22][1,13,22][1,14,22][1,15,22][1,16,22][1,17,18,22][1,17,19,22][1,17,20,22][1,17,21,22]

### Edge-Pair Coverage
#### Edge-Pair Test Requirements
[1,2,22],[1,2,22],[1,3,22],[1,4,22],[1,5,22],[1,6,22],[1,7,22],[1,8,22],[1,9,22],[1,10,22],[1,11,22],,[1,12,22],[1,13,22],[1,14,22],[1,15,22],[1,16,22],[1,17,18],[1,17,19],
[1,17,20],[1,17,21],[17,18,22],[17,19,22],[17,2022],[17,21,22]

#### Edge-Pair Test Paths
[1,2,22][1,3,22][1,4,22][1,5,22][1,6,22][1,7,22][1,8,22][1,9,22][1,10,22][1,11,22][1,12,22][1,13,22][1,14,22][1,15,22][1,16,22][1,17,18,22][1,17,19,22][1,17,20,22][1,17,21,22]


## EFG Graph

![EFG drawio](https://github.com/SOEN345-WINTER2024/cfg-graph-lab-j3rrimmy/assets/98069409/a18f975e-cc4b-45ab-9164-8406e3c8c14f)


# Antimine-Android-Main
## Method 
    private fun listenToPurchase() {
        if (!preferenceRepository.isPremiumEnabled() && iapHandler.isEnabled()) {
            lifecycleScope.launch {
                iapHandler.listenPurchase().collect {
                    if (it) {
                        recreate()
                    }
                }
            }
        }
    }
## CFG Graph
<img width="338" alt="Screen Shot 2024-03-15 at 3 37 08 PM" src="https://github.com/SOEN345-WINTER2024/cfg-graph-lab-j3rrimmy/assets/98069409/4b577d92-cd81-40ff-a4e4-de47a80a82ef">


### Node Coverage
#### Node Test Requirements
[1][2][3][4]

#### Node Test Paths
[1,2,3,4]

### Edge Coverage
#### Edge Test Requirements 
[1,2][2,3][3,4]

#### Edge Test Paths
[1,2,3,4]

### Edge-Pair Coverage
#### Edge-Pair Test Requirements
[1,2,3][2,3,4]

#### Edge-Pair Test Paths
[1,2,3,4]

## EFG Graph
<img width="160" alt="Screen Shot 2024-03-15 at 3 42 08 PM" src="https://github.com/SOEN345-WINTER2024/cfg-graph-lab-j3rrimmy/assets/98069409/f1005105-d0aa-4de5-87a4-4b5dac502502">

