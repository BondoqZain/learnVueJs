<template>
    <div class="upper-footer">
        <div>
            <div><img src="../assets/Logo-light.png" alt="logo" /></div>
            <div>
                <p>
                    Empowering individuals to unlock their full<br />
                    potential through world-class education from<br />
                    industry leaders.
                </p>
            </div>
            <div>
                <a href="#"><i class="fa-brands fa-facebook"></i></a>
                <a href="#"> <i class="fa-brands fa-square-twitter"></i></a>
                <a href="#"> <i class="fa-brands fa-instagram"></i></a>
                <a href="#"> <i class="fa-brands fa-linkedin"></i></a>
            </div>
        </div>

        <div class="menu">
            <div>
                <span>courses</span>
                <ul>
                    <li>brouse all</li>
                    <li>business</li>
                    <li>marketing</li>
                    <li>technology</li>
                    <li>leadership</li>
                </ul>
            </div>

            <div>
                <span>company</span>
                <ul>
                    <li>about us</li>
                    <li>instructors</li>
                    <li>careers</li>
                    <li>press</li>
                    <li>blog</li>
                </ul>
            </div>

            <div>
                <span>support</span>
                <ul>
                    <li>help center</li>
                    <li>contact</li>
                    <li>terms</li>
                    <li>privacy</li>
                    <li>cookies</li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scoped>
p {
  font-family: Montserrat Alternates;
  font-weight: 400;
  font-size: 16px;
  line-height: 27.2px;
  letter-spacing: -0.31px;
  color: var(--white-muted);
}

a {
  color: var(--white-muted);
  gap: 2rem;
}

.upper-footer {
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
    justify-content: space-evenly;
    border-bottom: 1px solid var(--divider);
    padding-bottom: 20px;
    margin-bottom: 20px;
}

.menu {
    display: flex;
    width: 50%;
    justify-content: space-between;
}

.menu span {
    font-family: Montserrat Alternates;
    font-weight: 700;
    font-style: Bold;
    font-size: 14px;
    line-height: 20px;
    letter-spacing: 1.95px;
    text-transform: uppercase;
    color: var(--white);
}

.menu ul {
    padding: 0;
    margin-bottom: 15px;
    text-align: left;
}

.menu ul li {
    font-family: Montserrat Alternates;
    font-weight: 400;
    font-size: 14px;
    line-height: 20px;
    letter-spacing: -0.15px;
    text-transform: capitalize;
    list-style: none;
    margin: 10px auto;
    text-align: left;
    color: var(--white-muted);
}
</style>