*************************************************

1- npx create-near-app todo

2- yarn install

3- yarn dev

4- yarn build:release

5- near dev-deploy 


or run ./scripts/build.sh instead of 4,5



*************************************************

near view dev-1645429298908-23414589644047 hello

near call dev-1645429298908-23414589644047 greetingUser --account_id tilek.testnet 

near call dev-1645429298908-23414589644047 showMyQuestions --account_id tilek.testnet
near call dev-1645429298908-23414589644047 showMyAnswers --account_id tilek.testnet 

near call dev-1645429298908-23414589644047 addQuestion '{"question":"What is a sharding?"}' --account_id tilek.testnet
near call dev-1645429298908-23414589644047 addQuestion '{"question":"What is WEB 3?"}' --account_id tilek.testnet
near call dev-1645429298908-23414589644047 addAnswer '{"answer":"Sharding does a horizontal partition of your database and turns into smaller, more manageable tables."}' --account_id tilek.testnet
near call dev-1645429298908-23414589644047 addAnswer '{"answer":"Web 3.0 is a general idea for a decentralized Internet based on public blockchains"}' --account_id tilek.testnet

near call dev-1645429298908-23414589644047 deleteQuestion '{"question":1}' --account_id tilek.testnet
near call dev-1645429298908-23414589644047 deleteAnswer '{"answer":1}' --account_id tilek.testnet

near call dev-1645429298908-23414589644047 showMyQuestions --account_id tilek.testnet
near call dev-1645429298908-23414589644047 showMyAnswers --account_id tilek.testnet 

near call dev-1645429298908-23414589644047 getNumQuestions --account_id tilek.testnet
near call dev-1645429298908-23414589644047 getNumAnswers --account_id tilek.testnet 



--------------------------------------------------------------------------------------------

yarn test:unit