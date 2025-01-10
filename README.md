# TRUEHN-GOLD
TRUEHN GOLD [TRUEHNG]

Issuers : AFM / EC / SR 

By Human Nature 4 Human Nature 

/**
 *Submitted for verification at coin Market cap ![Screenshot_20250103-192055](https://github.com/user-attachments/assets/622c6102-19a1-4503-b415-fb3917f19af9)
![IMG-20241202-WA0027](https://github.com/user-attachments/assets/04de402b-e88f-4d97-b01d-9264daedcce1)
![IMG-20250105-WA0031](https://github.com/user-attachments/assets/3079af92-42f1-429a-a1c7-51047de278fa)
.com on 2025-01-10
*/

pragma solidity ^0.8.3;

contract Token {
    mapping(address => uint) public balances;
    mapping(address => mapping(address => uint)) public allowed;
    uint public totalSupply;
    string public name;
    string public symbol;
    uint public decimals;
    
    event Transfer(address indexed from, address indexed to, uint value);
    event Approval(address indexed owner, address indexed spender, uint value);
    
    constructor(string memory _name, string memory _symbol, uint _dec, uint _supply, address _owner) {
        name = _name;
        symbol = _symbol;
        decimals = _dec;
        totalSupply = _supply * 10 ** decimals;
        balances[_owner] = totalSupply;
        emit Transfer(address(0), _owner, totalSupply);
    }
    
    function balanceOf(address owner) public view returns(uint) {
        return balances[owner];
    }
    
    function transfer(address to, uint value) public returns(bool) {
        require(balances[msg.sender] >= value, 'balance too low');
        balances[to] += value;
        balances[msg.sender] -= value;
        emit Transfer(msg.sender, to, value);
        return true;
    }
    
    function transferFrom(address from, address to, uint value) public returns(bool) {
        require(balances[from] >= value, 'balance too low');
        require(allowed[from][msg.sender] >= value, 'allowance too low');
        balances[to] += value;
        balances[from] -= value;
        allowed[from][msg.sender] -=value;
        emit Transfer(from, to, value);
        return true;   
    }
    
    function approve(address spender, uint value) public returns (bool) {
        allowed[msg.sender][spender] = value;
        emit Approval(msg.sender, spender, value);
        return true;   
    }
    
    function allowance(address owner, address spender) public view returns (uint) {
        return allowed[owner][spender];
    }
    
}
https://www.perplexity.ai/search/coin-market-cap-truehn-gold-pr-vf0CLJtMQz.QjAYhzbXToQevent Transfer(address indexed from, address indexed to, uint value);
event Approval(address indexed owner, address indexed spender, uint value);

constructor(string memory _name, string memory _symbol, uint _dec, uint _supply, address _owner) {
    name = _name;
    symbol = _symbol;
    decimals = _dec;
    totalSupply = _supply * 10 ** decimals;
    balances[_owner] = totalSupply;
    emit Transfer(address(0), _owner, totalSupply);
}

function balanceOf(address owner) public view returns(uint) {
    return balances[owner];
}

function transfer(address to, uint value) public returns(bool) {
    require(balances[msg.sender] >= value, 'balance too low');
    balances[to] += value;
    balances[msg.sender] -= value;
    emit Transfer(msg.sender, to, value);
    return true;
}

function transferFrom(address from, address to, uint value) public returns(bool) {
    require(balances[from] >= value, 'balance too low');
    require(allowed[from][msg.sender] >= value, 'allowance too low');
    balances[to] += value;
    balances[from] -= value;
    allowed[from][msg.sender] -=value;
    emit Transfer(from, to, value);
    return true;   
}

function approve(address spender, uint value) public returns (bool) {
    allowed[msg.sender][spender] = value;
    emit Approval(msg.sender, spender, value);
    return true;   
}

function allowance(address owner, address spender) public view returns (uint) {
    return allowed[owner][spender];
}event Transfer(address indexed from, address indexed to, uint value);
event Approval(address indexed owner, address indexed spender, uint value);

constructor(string memory _name, string memory _symbol, uint _dec, uint _supply, address _owner) {
    name = _name;
    symbol = _symbol;
    decimals = _dec;
    totalSupply = _supply * 10 ** decimals;
    balances[_owner] = totalSupply;
    emit Transfer(address(0), _owner, totalSupply);
}

function balanceOf(address owner) public view returns(uint) {
    return balances[owner];
}

function transfer(address to, uint value) public returns(bool) {
    require(balances[msg.sender] >= value, 'balance too low');
    balances[to] += value;
    balances[msg.sender] -= value;
    emit Transfer(msg.sender, to, value);
    return true;
}

function transferFrom(address from, address to, uint value) public returns(bool) {
    require(balances[from] >= value, 'balance too low');
    require(allowed[from][msg.sender] >= value, 'allowance too low');
    balances[to] += value;
    balances[from] -= value;
    allowed[from][msg.sender] -=value;
    emit Transfer(from, to, value);
    return true;   
}

function approve(address spender, uint value) public returns (bool) {
    allowed[msg.sender][spender] = value;
    emit Approval(msg.sender, spender, value);
    return true;   
}

function allowance(address owner, address spender) public view returns (uint) {
    return allowed[owner][spender];
}event Transfer(address indexed from, address indexed to, uint value);
event Approval(address indexed owner, address indexed spender, uint value);

constructor(string memory _name, string memory _symbol, uint _dec, uint _supply, address _owner) {
    name = _name;
    symbol = _symbol;
    decimals = _dec;
    totalSupply = _supply * 10 ** decimals;
    balances[_owner] = totalSupply;
    emit Transfer(address(0), _owner, totalSupply);
}

function balanceOf(address owner) public view returns(uint) {
    return balances[owner];
}

function transfer(address to, uint value) public returns(bool) {
    require(balances[msg.sender] >= value, 'balance too low');
    balances[to] += value;
    balances[msg.sender] -= value;
    emit Transfer(msg.sender, to, value);
    return true;
}

function transferFrom(address from, address to, uint value) public returns(bool) {
    require(balances[from] >= value, 'balance too low');
    require(allowed[from][msg.sender] >= value, 'allowance too low');
    balances[to] += value;
    balances[from] -= value;
    allowed[from][msg.sender] -=value;
    emit Transfer(from, to, value);
    return true;   
}

function approve(address spender, uint value) public returns (bool) {
    allowed[msg.sender][spender] = value;
    emit Approval(msg.sender, spender, value);
    return true;   
}

function allowance(address owner, address spender) public view returns (uint) {
    return allowed[owner][spender];
}event Transfer(address indexed from, address indexed to, uint value);
event Approval(address indexed owner, address indexed spender, uint value);

constructor(string memory _name, string memory _symbol, uint _dec, uint _supply, address _owner) {
    name = _name;
    symbol = _symbol;
    decimals = _dec;
    totalSupply = _supply * 10 ** decimals;
    balances[_owner] = totalSupply;
    emit Transfer(address(0), _owner, totalSupply);
}

function balanceOf(address owner) public view returns(uint) {
    return balances[owner];
}

function transfer(address to, uint value) public returns(bool) {
    require(balances[msg.sender] >= value, 'balance too low');
    balances[to] += value;
    balances[msg.sender] -= value;
    emit Transfer(msg.sender, to, value);
    return true;
}

function transferFrom(address from, address to, uint value) public returns(bool) {
    require(balances[from] >= value, 'balance too low');
    require(allowed[from][msg.sender] >= value, 'allowance too low');
    balances[to] += value;
    balances[from] -= value;
    allowed[from][msg.sender] -=value;
    emit Transfer(from, to, value);
    return true;   
}

function approve(address spender, uint value) public returns (bool) {
    allowed[msg.sender][spender] = value;
    emit Approval(msg.sender, spender, value);
    return true;   
}

function allowance(address owner, address spender) public view returns (uint) {
    return allowed[owner][spender];
}event SwapTruehnGoldForBTC(address indexed user, uint256 truehnGoldAmount, uint256 btcAmount);
event SwapTruehnGoldForUSDT(address indexed user, uint256 truehnGoldAmount, uint256 usdtAmount);
event SwapBTCForTruehnGold(address indexed user, uint256 btcAmount, uint256 truehnGoldAmount);
event SwapUSDTForTruehnGold(address indexed user, uint256 usdtAmount, uint256 truehnGoldAmount);
