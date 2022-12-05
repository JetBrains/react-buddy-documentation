## Preview configuration (DevSupport)


### Using with Refine

```

function AppLayout({...props}) {
  return (
      <DevSupport ComponentPreviews={ComponentPreviews}
                  useInitialHook={useInitial}
      >
        <Layout {...props}/>
      </DevSupport>
  )
}

function App() {

  return (
    <Refine
      Layout={AppLayout}
      // other props  
    />
  );
}


