countTotalProds = db.produtos.count();
db.resumoProdutos.insertOne({
  franquia: "McDonalds",
  totalProdutos: countTotalProds,
});

db.resumoProdutos.find(
  {},
  { _id: 0 },
);