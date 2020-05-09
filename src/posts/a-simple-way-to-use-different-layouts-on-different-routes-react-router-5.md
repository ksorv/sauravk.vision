---
layout: layouts/post.njk
title: A simple way to use different layouts on different routes, React Router 5
metaTitle: A simple way to use different layouts on different routes, React Router 5
metaDesc: A simple way to use different layouts on different routes, React Router 5
date: 2020-05-09T15:46:55.194Z
tags:
  - react
  - router
  - react router 5
  - layouts
---
Simply use:

```
<Route exact path={[
                  Routes.HOME,
                  Routes.EXPLORE,
                ]}
        >
        <Root>
          <SideBar isOpen={isSideBarOpen} sideBarRef={sideBarRef} />
          <Switch>
            <Route exact path={Routes.HOME} component={Home} />
            <Route exact path={Routes.EXPLORE} component={Explore} />
            <Route exact path={Routes.NOTFOUND} component={NotFound} />
            <Route component={NotFound} />
          </Switch>

          <UserSuggestions pathname={location.pathname} />
        </Root>
      </Route>
       <Route exact path={[Routes.SchoolStudents, Routes.SchoolCurriculum]}>
        <Switch>
          <Route
            exact
            path={Routes.SchoolStudents}
            component={SchoolStudents}
          />

          <Route
            exact
            path={Routes.SchoolCurriculum}
            component={SchoolCurriculum}
          />
        </Switch>
      </Route>
```