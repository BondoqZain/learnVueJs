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

            <div class="socials">
                <a href="#"><i class="fa-brands fa-facebook"></i></a>
                <a href="#"><i class="fa-brands fa-square-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-instagram"></i></a>
                <a href="#"><i class="fa-brands fa-linkedin"></i></a>
            </div>
        </div>

        <div class="menu">
            <div>
                <span>courses</span>
                <ul>
                    <li><a href="#">browse all</a></li>
                    <li><a href="#">business</a></li>
                    <li><a href="#">marketing</a></li>
                    <li><a href="#">technology</a></li>
                    <li><a href="#">leadership</a></li>
                </ul>
            </div>

            <div>
                <span>company</span>
                <ul>
                    <li><a href="#">about us</a></li>
                    <li><a href="#">instructors</a></li>
                    <li><a href="#">careers</a></li>
                    <li><a href="#">press</a></li>
                    <li><a href="#">blog</a></li>
                </ul>
            </div>

            <div>
                <span>support</span>
                <ul class="support-list">
                    <li><a href="#">help center</a></li>
                    <li><a href="#">contact</a></li>
                    <li><a href="#">terms</a></li>
                    <li><a href="#">privacy</a></li>
                    <li><a href="#">cookies</a></li>
                </ul>
            </div>
        </div>
    </div>
</template>
<style scoped>
.upper-footer {
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
    justify-content: space-between;
    border-bottom: 1px solid var(--divider);
    padding-bottom: 20px;
    margin-bottom: 20px;
}

.upper-footer > div:first-child {
    flex: 1 1 250px; 
}

.menu {
    display: flex;
    flex: 2 1 400px;
    flex-wrap: wrap;
    gap: 2rem;
    justify-content: space-between;
}

.menu > div {
    flex: 1 1 150px; 
}

.menu ul {
    padding: 0;
    list-style: none;

    display: flex;
    flex-direction: column;
    gap: 0.8rem;
}
span {
    color: var(--white);
    font-family: Montserrat Alternates;
    font-size: 14px;
    letter-spacing: -0.15px;
    text-transform: capitalize;
}
.menu ul li a {
    color: var(--white-muted);
    text-decoration: none;
    font-family: Montserrat Alternates;
    font-size: 14px;
    letter-spacing: -0.15px;
    text-transform: capitalize;
}

.menu ul li a:hover {
    color: var(--white);
}

.socials {
    display: flex;
    gap: 1rem;
    margin-top: 1rem;
}

.socials a {
    color: var(--white-muted);
    font-size: 18px;
}

p {
  font-family: Montserrat Alternates;
  font-size: 16px;
  line-height: 27.2px;
  letter-spacing: -0.31px;
  color: var(--white-muted);
}

@media (max-width: 768px) {
    .upper-footer {
        flex-direction: column;
        align-items: flex-start;
    }

    .menu {
        width: 100%;
        justify-content: flex-start;
    }
}
</style>