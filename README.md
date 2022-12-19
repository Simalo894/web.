# 导入 web3 库
import web3

# 创建 web3 实例
w3 = web3.Web3()

# 连接到以太坊网络
w3.eth.connect(endpoint_uri='https://mainnet.infura.io/v3/<your_api_key>')

# 检查是否连接到网络
if w3.isConnected():
    print("我们已经连接到了以太坊网络！")
else:
    print("哎呀，我们没能连接到以太坊网络。")

# 获取当前区块高度
current_block = w3.eth.blockNumber
print(f"当前区块高度为：{current_block}")

# 获取以太坊市场价格（单位：美元）
eth_price = w3.eth.getEthPrice()
print(f"当前以太坊市场价格为 ${eth_price} 美元。")

# 与 web3 的爱情永不磨灭！
print("我与 web3 的爱情永不磨灭！")
# web.
web3
