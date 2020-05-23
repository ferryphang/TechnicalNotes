1. Inject Props dan menggunakan props didalam component

```
<App data={1}>

class App extends Component {
	constructor(props){
		super(props)

		this.props = props
	}
}
```

2.SetState bisa diberikan param tambahan

```
this.setState({data: "Hello"})

this.setState((prevState,prevProps) => {
	return prevState(data: prevProps.data)
}, console.log("Setelah selesai diatas baru panggil ini"))


3. LifeCycle Class Component

MOUNTING PHASE
Selalu jalan yang pertama kali
```

constructor(){}

```
Kemudian render akan berjalan
```

render(){}

```
Class selesai terinisiasi
```

componenDidMount(){}

```
UPDATING PHASE
apabila ada props atau state berubah dan menentukan apakah perlu dirender ulang atau ga dgn mengirimkan true atau false
```

shouldComponentUpdate(nextProps, nextState){}

```

Invoke saat setelah shouldComponentUpdate terjadi
```

componenDidUpdate()

```

```

4. Kalau terjadi masalah pada dependency saat running app

```
...,
	{ resolution: {
			"nama_package": versi
	}}
``
```
