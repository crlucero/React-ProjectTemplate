### Description
 This is a boiler plate template for any React Project. 

 ## Setup/Installation Requirements to run program
 - Clone from Github

- Navigate to root project directory in the terminal.

- Run npm install into the terminal to install dependancies.

- Npm run start to launch project in browser

- Add more dependencies and rules as you wish to use in your project

#### Install Routing (if needed)
- import ' import { HashRouter } from 'react-router-dom'; ' into index.jsx
- Wrap App component's JSX Tags in <HashRouter> tags to ensure all children of App have access to routing capabilities. 
    const render = (Component) => {
    ReactDOM.render(
        <AppContainer>
        <HashRouter>
            <Component/>
        </HashRouter>
        </AppContainer>,
        document.getElementById('react-app-root')
    );
    };
- Import ' import { Switch, Route } from 'react-router-dom'; ' into App.jsx
- Define routes within <Switch> tags
    Example:
        function App(){
            return (
                <div>
                <Header/>
                <Switch>
                    <Route exact path='/' component={TicketList} />
                </Switch>
                </div>
            );
        }