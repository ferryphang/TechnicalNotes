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
